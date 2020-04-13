<template>
    <section class="resume-section p-3 p-lg-5 d-flex justify-content-center" id="experience">
      <div class="w-100">
        <h2 class="mb-5">Experiencia</h2>

        <div class="resume-item d-flex flex-column flex-md-row justify-content-between mb-5" v-for="(obj,key) in experienceJSON" :key="key">
          <div class="resume-content">
            <h3 class="mb-0">{{obj.title}}</h3>
            <div class="subheading mb-3" style="color:#909497">{{obj.institution}}</div>
            <p>{{obj.description}}</p>
          </div>
          <div class="resume-date text-md-right">
            <span class="text-primary">{{obj.date}}</span>
          </div>
        </div>
      </div>

    </section>

    
</template>

<script>
export default {
    data: () =>({
        experienceJSON:[
            {
                title:'Desarrollador web',
                institution:'Aconsa s.a de c.v',
                description:'Luego de un año aprendiendo acerca de .Net, especifícamente .Net Framework con el patrón MVC se presentó la oportunidad de brindar una solución que permitiera agilizar los procesos de la empresa a partir de un sistema web, luego de iniciar como pasante junto a un grupo de colegas que en poco tiempo se hicieron muy cercanos ♥ finalmente ocupé el cargo de desarrollador web lo que para mí significó el inicio de mi carrera y un camino el cual me permite aprender cosas distintas cada día.',
                date: 'Octubre 2019 - Actualmente'
            },
            {
                title:'Diseñador web',
                institution:'CABO MULTISERVICIOS',
                description:'De aquí creció mi interes por el front-end, realicé mi primera página web y fue mi primer proyecto freelance, salí de mi zona de confort y empecé a explorar frameworks de javascript, me incliné por Vue.js luego Nuxt.js (un framework de un framework)...Este portafolio está hecho con Vue.js ♥',
                date: 'Noviembre 2019'
            }
        ]
    })
}
</script>