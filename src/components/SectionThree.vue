<template>
    <div class="container-fluid">
        <div class="row faq-header-section">
            <p class="faq-par">Frequently Asked Questions</p>
        </div>
        <div class="row faq-body-section">
            <div class="col-3">
                <p class="faq-body-left-section-par1">Do you have any question?<br>Please ask here we ready to<br>support</p>
                <p class="faq-body-left-section-par2">If your question is not list here,<br>please feel free to make a<br>manual support.</p>
                <div class="faq-body-left-section-btn">
                    <a>Ask your Question</a>
                </div>
            </div>
            <div class="col-8">
                <ul>
                    <li v-for="(navItem, i) in menuList" :key="i" class="nav-item">
                        <a class="nav-link" href="javascript:;" data-toggle="collapse" role="button" :aria-expanded="navItem.expand" @click.prevent="navItemCollapse(i)">
                            <i class="ni ni-single-copy-04 text-primary"></i>
                            <span class="nav-link-text">{{ navItem.question }}</span>
                            <span :class="'arrow '+[navItem.expand ? 'down' : 'right']"></span>
                        </a>
                        <div v-if="navItem.answer" class="collapse" :class="{show: navItem.expand}">
                            <ul class="nav nav-sm flex-column">
                                <span class="nav-link">{{ navItem.answer }}</span>
                            </ul>
                        </div>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionFour',
    data() {
    return {
      menuList: [{
          question: 'How much does it cost to be 365 member?',
          expand: true,
          answer: 'For our recent trip to S.A. I booked several accommodation thru SA Places. I just wanted to tell you that everything worked out perfectly with all the bookings and also your booking was very quick and professional. I hope I have the opportunity to re-visit South Africa soon, I will then make my bookings with your company again. I will also recommend'
        },
        {
          question: 'How can I join as an influencer?',
          expand: false,
          answer: 'For our recent trip to S.A. I booked several accommodation thru SA Places. I just wanted to tell you that everything worked out perfectly with all the bookings and also your booking was very quick and professional. I hope I have the opportunity to re-visit South Africa soon, I will then make my bookings with your company again. I will also recommend'
        },
        {
          question: 'What are the prizes for the daily playing?',
          expand: false,
          answer: 'For our recent trip to S.A. I booked several accommodation thru SA Places. I just wanted to tell you that everything worked out perfectly with all the bookings and also your booking was very quick and professional. I hope I have the opportunity to re-visit South Africa soon, I will then make my bookings with your company again. I will also recommend'
        },
        {
          question: 'Can I make cash payments?',
          expand: false,
          answer: 'For our recent trip to S.A. I booked several accommodation thru SA Places. I just wanted to tell you that everything worked out perfectly with all the bookings and also your booking was very quick and professional. I hope I have the opportunity to re-visit South Africa soon, I will then make my bookings with your company again. I will also recommend'
        },
        {
          question: 'How do I get the payment complete?',
          expand: false,
          answer: 'For our recent trip to S.A. I booked several accommodation thru SA Places. I just wanted to tell you that everything worked out perfectly with all the bookings and also your booking was very quick and professional. I hope I have the opportunity to re-visit South Africa soon, I will then make my bookings with your company again. I will also recommend'
        }
      ]
    }
  },
  methods: {
    navItemCollapse(index) {
      this.menuList = this.menuList.map((item, i) => {
        item.expand = !item.expand
        if (i !== index) {
          item.expand = false
        }
        return item
      })
    }
  }
};
</script>

<style scoped>
.container-fluid {
    min-width: 100vh;
    background-color: black;
    background-repeat: no-repeat;
    color: #ffffff;
}

.faq-header-section {
    text-align: center;
}

.faq-par {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 800;
    font-size: 65px;
    letter-spacing: -1.5px;
    color: #FDFDFD;
}

.faq-body-section {
    text-align: left;
    margin-top: 100px;
    margin-left: 80px;
}

.faq-body-left-section-par1 {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: bold;
    font-size: 24px;
    line-height: 34px;
    letter-spacing: -1px;
    color: #FFFFFF;
    margin-bottom: 30px;
}

.faq-body-left-section-par2 {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: normal;
    font-size: 16px;
    line-height: 26px;
    color: #CDCADB;
    margin-bottom: 40px;
}

.faq-body-left-section-btn {
    cursor: pointer;
    max-width: 194px;
    color: #ffffff !important;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: bold;
    font-size: 15px;
    color: white;
    text-align: center;
    letter-spacing: -0.16px;
    clip-path: polygon(0 0, 91% 0, 100% 26%, 100% 80%, 100% 100%, 0 100%, 0% 80%, 0 24%);
    border-style: solid;
    border-width: 2px;
    border-image: linear-gradient(180deg, #9672FF 0%, #6B4FE8 100%) 1;
    border-radius: 5px;
    padding-top: 15px;
    padding-bottom: 15px;
    text-decoration: none !important;
}

.faq-body-left-section-btn:hover {
    background: linear-gradient(180deg, #9672FF 0%, #6B4FE8 100%);
}

ul li {
    list-style-type: none;
}

.nav-item {
    border-bottom: 1px solid #9672FF;
}

.nav-link-text {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 500;
    font-size: 17px;
    line-height: 35px;
    letter-spacing: -0.2px;
    color: #FFFFFF;
    padding-bottom: 10px !important;
}

.nav-link {
    font-family: Poppins;
    font-style: normal;
    font-weight: normal;
    font-size: 16px;
    line-height: 30px;
    color: #FFFFFF;
    opacity: 0.7;
    text-decoration: none;
    padding-left: 0px;
    padding-right: 0px;
    padding-bottom: 30px;
}

.nav-link:hover {
    color: #FFFFFF !important;
    opacity: 0.7;
}

.arrow {
    border: solid white;
    border-width: 0 3px 3px 0;
    padding: 3px;
    float: right;
    margin-right: 20px;
    margin-top: 1%;
}

.right {
    transform: rotate(-45deg);
    -webkit-transform: rotate(-45deg);
}

.down {
    transform: rotate(45deg);
    -webkit-transform: rotate(45deg);
}
</style>