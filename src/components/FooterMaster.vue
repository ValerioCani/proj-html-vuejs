<template>
  <footer>
    <div class="container flex">

      <div class="footer_column">
          <h2>{{About.headline}}</h2>
          <p>{{About.content}}</p>
          <i v-for="(icon, index) in About.social" :key="index" class="fa-brands" :class="'fa-'+icon"></i>
      </div>

      <div class="footer_column">
          <h2>{{Contact.headline}}</h2>
          <p v-for="(contact, index) in Contact.content" :key="index">{{contact}}</p>
      </div>

      <div class="footer_column">
          <h2>{{Pages.headline}}</h2>
          <ul>
            <li v-for="(page, index) in Pages.content" :key="index">{{page}}</li>
          </ul>
      </div>

      <div class="footer_column">
          <h2>{{Blog.headline}}</h2>
          <div v-for="(article, index) in Blog.content" :key="index">
            <img :src="require('@/assets/img/' + article.img)" alt="">
            <div>
              <p>{{article.text}}</p>
              <span>{{article.date}}</span>
            </div>
          </div>
      </div>

    </div>
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
            img:'Article1.jpeg',
            text:'Our main target is to "Developing Yourself as a Leader"',
            date:'--August 9, 2018',
          },
          {
            img:'Article2.jpeg',
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
@import '@/assets/styles/var.scss';
footer{
  background-color: $primary_color;
  .footer_column{
    
  }
}
</style>