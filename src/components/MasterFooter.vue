<template>
  <footer>
    <div class="container"></div>
  </footer>
</template>

<script>
export default {
  name:'MasterFooter',
  data(){
    return{   

      About:{
        headline:'ABOUT',
        content:'Masterstudy is Educatio WordPres Theme Featured By Learning Management System (LMS) for online education. Developed by StylemixThemes.',
        social:[
          'facebook',
          'twitter',
          'instagram'
        ]
      },

      Contact:{
        headline:'CONTACT',
        content:[
          'USA, California 20, First Avenue, California',
          'Tel.: +1 212 458 300 32',
          'Fax: +1 212 375 24 14',
          'info@masterstudy.com'
        ]
      },
      
      Pages:{
        headline:'PAGES',
        content:[
        'Blog',
        'Courses',
        'Home',
        'Membership',
        'Shortcodes',
        'Typography',
        ]
      },

      Blog:{
        headline:'BLOG',
        content:[
          {
            img:'',
            text:'Our main target is to "Developing Yourself as a Leader"',
            date:'--August 9, 2018',
          },
          {
            img:'',
            text:'Those Other College Expenses You Aren\'t Thinking About',
            date:'--June 3, 2015',
          },
        ]
      }
    } 
  }
}
</script>

<style scoped lang="scss">

</style>