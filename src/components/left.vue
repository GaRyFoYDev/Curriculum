<template>
<div class="left_container">

<div class="left_header">
    <h2>Gary <span>FOY</span></h2>
    <h3 class="job">Développeur fullstack</h3>
</div>

<div class="left_contact">
    <div class="left_contact_icons">
        <i class="fa-solid fa-phone"></i>
        <i class="fa-solid fa-envelope"></i>
        <i class="fa-solid fa-house-chimney"></i>
        <i class="fa-brands fa-github"></i>
    </div>
    <div class="left_contact_text">
        <a href="callto:+33652252438">+33 6 52 25 24 38</a>
        <a href="mailto:garyfoy@hotmail.fr" >garyfoy@hotmail.fr</a>
        <p>3 Allée Maurice Ravel 92260 Fontenay-aux-Roses</p>
        <a href="https://github.com/GaryOpenClassroom">github.com/GaryOpenClassroom</a>

    </div>
    
</div>


<div class="left_profil">
   <h3>présentation</h3>
   <p>Bonjour, je suis Gary FOY, développeur fullstack en reconversion professionelle. <br>
    Je sors de 7 années d'entrepreneuriat où j'ai dirigé un camion food-truck avec ma compagne. <br>
    La crise du covid nous a permis de revoir nos priorités et de profiter de notre fils, et nous avons décidé
    de la fermeture de notre entreprise bien que florissante.<br>
    J'ai entamé une formation de développeur chez Openclassrooms qui m'a permise en réalisant des projets 
    professionnels, en effectuant des recherches Google et en lisant la documentation disponibles d'acquérir 
    les compétences de bases nécéssaires à tout bon dévellopeur.<br>
    Désormais, je recherche un premier emploi de dévellopeur frontend ou fullstack afin de continuer à monter en compétences.
     
   </p>
   
    
</div>
<div class="left_experience">
   <h3>expériences</h3>
   <h4>Développeur fullstack - 2022</h4>
   <h4>Openclassroom / full remote</h4>
   <p>La vidéo ci-dessous représente, le dernier projet de ma formation chez Openclassrooms. <br>
    Il s'agit d'un réseau social d'entreprise, où j'ai dû implémenter le backend et le frontend de l'application web.<br>
    J'ai mis en place un CRUD pour les utilisateurs, les publications et les commentaires , mais aussi système d'authentification à l'aide des JWT tokens.<br>
    Cette application a été développeur avec nodeJS, express, sequelize, mySQL (backend), vueJs pinia et vue router (frontend).
    Vous pouvez retrouver l'intégralité de mes travaux sur ma page  <a href="https://github.com/GaryOpenClassroom">github.com</a>


    
    
    </p>
   
   <video src="" controls></video>
    
</div>

</div>
</template>


<style lang="scss" scoped>


.left{

    &_container{
        width: 55%;
        background-color: var(--grey-2);
        display: flex;
        flex-direction:column;
        padding: 40px;
        gap:50px;

    @media screen and (max-width: 768px) {
        width: 100%;
        padding: 30px ;
        align-items: center;
}
    
    }

    &_contact{
        display: flex;
        align-items: center;
      


     
        &_icons{
            display: flex;
            flex-direction: column;
            gap: 10px;
            color: var(--primary-1);
            border: 2px solid var(--primary-1);
            border-radius: 20px;
            margin-right: 10px;
            padding: 10px 5px;
        }

        &_text{
            display: flex;
            flex-direction: column;
             gap: 10px;
             color: var(--grey-3);
             position: relative;

                a{
                 color: var(--grey-3); 
             }

        }


    }

}

h2{
    font-size: 2.5rem;
  
}
h3{
    color: var(--primary-1);
    margin-bottom: 20px;
     letter-spacing: 3px;
}
h4{
   
    margin-bottom: 10px;
    text-transform: capitalize;
}

p{
    text-align: justify;
}

span{
    font-weight: 500;
    color: var(--primary-1);
}

p{
    line-height: 30px;
}




video{
    display: block;
    margin: 30px auto;
    width: 100%;
    min-height:300px;
    ;
}



.job{
    font-weight: 100;
    color: var(--text-color)
}

</style>