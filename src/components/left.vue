<template>
<div class="left_container">

<div class="left_header">
    <h2>Gary <span>FOY</span></h2>
    <h3>Développeur fullstack</h3>
</div>

<div class="left_contact">
    <div class="left_contact_icons">
        <i class="fa-solid fa-phone"></i>
        <i class="fa-solid fa-envelope"></i>
        <i class="fa-solid fa-house-chimney"></i>
    </div>
    <div class="left_contact_text">
        <p>+33 6 52 25 24 38</p>
        <p>garyfoy@hotmail.fr</p>
        <p>3 Allée Maurice Ravel 92260 Fontenay-aux-Roses</p>

    </div>
    
</div>

</div>
</template>


<style lang="scss" scoped>


.left{

    &_container{
        width: 65%;
        background-color: var(--grey-2);
        display: flex;
        flex-direction:column;
        padding: 40px;

    @media screen and (max-width: 768px) {
        width: 100%;
        padding: 30px 0;
        align-items: center;
}
    
    }

    &_contact{
        display: flex;
        align-items: center;
        margin-top: 50px;

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
        }
    }

}

h2{
    font-size: 2.5rem;
  
}
h3{
    
    font-weight: 200;
}

span{
    font-weight: 500;
    color: var(--primary-1);
}

</style>