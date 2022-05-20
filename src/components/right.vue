<template>
<div class="right_container">
    <div class="right_image">
        <div class="right_image_container">
            <div class="right_image_center">
                <img src="../assets/images/thumbnail_IMG_3312.png" alt="photo de profil">
            </div>
            <div class="right_image_ball">
            </div>
        </div>
    </div>
    
    <div class="right_education">  
        <h3>formation</h3>

        <div v-for="education in educations" class="right_education_info">
            <p>{{education.year}}</p>
            <h4>{{education.name}}</h4>
            <p>{{education.school}} - {{education.city}}</p>
        </div>
        
    </div>
    <div class="right_langue">  
        <h3>langues</h3>
            <ul v-for="language in languages">
                <li>{{language.name}} - {{language.level}}</li>
            </ul>
    </div>
    <div class="right_skills">  
        <h3>compétences</h3>
        <div v-for="skill in skills" class="right_skills_container">
            <h4 class="right_skills_title">{{skill.name}}</h4>
            <div class="right_skills_progress">
                <div class="bar" :style="{width: skill.progress + '%'}"></div>
            </div>
        </div>
      
    </div>
</div>

</template>

<script setup lang="ts">

const skills = [

    { name:"html / css", progress: 90},
    { name:"javascript / vueJs", progress: 75},
    { name:"nodeJS / Express", progress: 70},
    { name:"MongoDB / MySQL", progress: 65}
]
const languages = [

    { name:"Anglais", level: "C1"},
    { name:"Portuguais brésilien", level: "B2"},
    { name:"Espagnol", level: "B1"},

    
]
const educations = [

    { name: "Baccalauréat Scientifique", year:"2007", level: "", school:"Lycée Jean Jaurès", city:"Montreuil"},
    { name: "Bachelor management entrepreneurial", year:"2010", level: "Bac + 3", school:"Novancia Business School", city:"Paris"},
    { name: "Développeur intégrateur web", year:"2022", level: "Bac + 2", school:"Openclassrooms", city:"Full remote"},  
]

</script>

<style lang="scss" scoped>

.right{
    
     &_container{
        display: flex;
        flex-direction: column;
        gap: 15px;
        width: 35%;
        height: 100%;
        padding: 40px;   
    }
    

    &_image{
            margin: 10px auto 20px;
            &_container{
                display: flex;
                justify-content: center;
                align-items: center;
                width: 180px;
                height: 180px;
                border: 2px solid var(--grey-1);
                border-top: 4px solid var(--primary-1) ;
                border-right: 4px solid var(--primary-1) ;
                border-radius: 50%;
                position: relative;
             
            }

            img{
                max-width: 100%;
                margin-top: -45px;
                margin-left: 10px ;
               
               
                border-radius: 50%;
            }


            &_center{
                display: flex;
                justify-content: center;
                align-items: center;
                width: 80%;
                height: 80%;
                background-color: var(--primary-1);
                border-radius: 50%;
            }
            &_ball{
                width: 10%;
                height: 10%;
                background-color: var(--primary-1);
                border-radius: 50%;
                position: absolute;
                left: 10px;
                bottom: 25px;
            }

          
    }
      &_education{

            &_info{
                margin-bottom: 15px;
            }
            &_info > *{
                margin-bottom: 3px;
            }
        }

    &_skills{

        &_container{
            margin-bottom: 20px;
        }

        &_title{
            margin-bottom:10px;
        }

        &_progress{
            width: 100%;
            background-color: var(--grey-1);
        }
    }
}
h3{
    color: var(--primary-1);
    margin-bottom: 20px;
    letter-spacing: 3px;
}
h4{
   
  
    text-transform: capitalize;
}

p{
    text-align: justify;
}

 
.bar{
    height: 10px;
    background-color: var(--primary-1);
}




</style>