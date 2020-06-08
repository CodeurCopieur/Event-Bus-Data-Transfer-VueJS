<template>
  <div class="wrapper__article">
    <article v-for="(item, index) in teaser" :key="index">
      <div class="teaser">
        <h2>{{ item.title }} </h2>
        <p> {{ item.text }}</p>
      </div>
  </article>
  </div>
</template>

<script>

export default {
  data () {
    return {
      teaser: [
        {
          title: 'Event Bus Data Transfer VueJS',
          text: 'Dans ce mini projet : il faut filtrer les articles en fonction du résultat de la recherche. Il y aura deux composants : - Navigation qui va contenir le composant menu et le composant de champ de re…'
        },
        {
          title: 'Components Data Transfer Vuejs',
          text: 'La communication entre un composant parent et un composant enfant est plus plutôt simple. Nous allons voir comment on peut transférer des données entre composants dans Vue JS '
        },
        {
          title: 'Vue Router Transition',
          text: 'Les transitions sont la touche finale lors de la conception d\'un site internet. Il faut combiner la bibliothèque vue router et de belle transition de page.'
        },
        {
          title: 'Vue Router Basics',
          text: 'Première utilisation de vue router. j\'utilise cette bibliothèque pour créer ma première SPA(Single Page Application). Elle permet de basculer entre les pages sans rafraîchissement de page, ce qui r… '
        },
        {
          title: 'Luigis Theme WordPress',
          text: 'Un site Web HTML statique convertir en monpropre thème WordPress. J\'utilise un plugin pratique pour WordPress appelé Advanced Custom Fields '
        },
        {
          title: 'AOS Animate On Scroll',
          text: 'Dans ce projet, j\'utilise la bibliothèque AOS (Animate on Scroll) pour implémenter un effet lorsque la page défile '
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.wrapper__article {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  article{
    width: calc(100%/3);
    margin: 20px;

    .teaser {
      background: rgb(59, 73, 223);
      color: #fff;
      padding: 10px;
      h2 {
        margin-bottom: 10px;
      }
    }
  }
}
</style>