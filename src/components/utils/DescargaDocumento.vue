<template>
    <div class="descarga-documento">
        <h5>{{titulo}}</h5>
        <p>{{autorxs}} </p>
        <a :href="ruta" target="_blank"><img :src='require("@/assets/img/iconos/descargar.svg")'/><span>Descarga {{formato}}</span></a>
        
    </div>
</template>

<script>
export default {
    name: 'DescargaDocumento',
    props:{
        titulo: String,
        autorxs: String,
        ruta: String,
        formato: String
    }
}
</script>

<style lang="scss">
.descarga-documento{
    width:100%;
    h5{
        color: #fff;
        font-size: 24px;
        font-weight: 600;
        margin:10px 0 ;
    }
    p{
        letter-spacing: 0.8px;
        color: #FFFFFF;
        text-transform: uppercase;
        font-size: 14px;
    }
    a{
        letter-spacing: 0.7px;
        color: #FDA1C9;
        text-transform: uppercase;
        opacity: 1;
        font-weight: 800;
        font-size: 14px;
        text-decoration: none;
        display: flex;
        img{
            margin-right: 10px;
            width: 18px;
        }
        span{
            line-height: 18px;
        }
    }
    padding-bottom: 24px;
    border-bottom: 1px solid #FFFFFF80;
    margin-bottom:30px;
}
</style>