<template>
    <section class="resume-section p-3 p-lg-5 d-flex align-items-center"  id="education">
      <div class="w-100">
        <h2 class="mb-5">Educación</h2>

        <div class="resume-item d-flex flex-column flex-md-row justify-content-between mb-5"  v-for="(obj,key) in educacionJSON" :key="key">
          <div class="resume-content">
            <h3 class="mb-0">{{obj.institution}}</h3>
            <div class="subheading mb-3" style="color:#909497">{{obj.title}}</div>
            <div>{{obj.description}}</div>
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
        educacionJSON:[
            {
                institution:'Universidad Gerardo Barrios',
                title:'Ingeniería de sistemas y redes informáticas',
                description:'"Realmente nunca es tarde para empezar de nuevo así como lo es para aprender sobre nuevos universos"',
                date: '2020'
            },
            {
                institution:'Colegio Tecnologico Cristiano',
                title:'Bachillerato General',
                description:'"that was fun."',
                date: '2016'
            }
        ]
    })
}
</script>