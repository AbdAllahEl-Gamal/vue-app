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
                    <li v-for="(item, index) in questionsAndAnswersList" :key="index" class="nav-item">
                        <a class="nav-link" data-toggle="collapse" role="button" :aria-expanded="item.expand" @click.prevent="itemCollapse(index)">
                            <span class="nav-link-question">{{ item.question }}</span>
                            <span :class="'arrow '+[item.expand ? 'down' : 'right']"></span>
                        </a>
                        <div v-if="item.answer" class="collapse" :class="{show: item.expand}">
                            <ul class="nav nav-sm flex-column">
                                <span class="nav-link answer">{{ item.answer }}</span>
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
      questionsAndAnswersList: [{
          question: 'How much does it cost to be 365 member?',
          answer: 'For our recent trip to S.A. I booked several accommodation thru SA Places. I just wanted to tell you that everything worked out perfectly with all the bookings and also your booking was very quick and professional. I hope I have the opportunity to re-visit South Africa soon, I will then make my bookings with your company again. I will also recommend',
          expand: false
        },
        {
          question: 'How can I join as an influencer?',
          answer: 'For our recent trip to S.A. I booked several accommodation thru SA Places. I just wanted to tell you that everything worked out perfectly with all the bookings and also your booking was very quick and professional. I hope I have the opportunity to re-visit South Africa soon, I will then make my bookings with your company again. I will also recommend',
          expand: false
        },
        {
          question: 'What are the prizes for the daily playing?',
          answer: 'For our recent trip to S.A. I booked several accommodation thru SA Places. I just wanted to tell you that everything worked out perfectly with all the bookings and also your booking was very quick and professional. I hope I have the opportunity to re-visit South Africa soon, I will then make my bookings with your company again. I will also recommend',
          expand: false
        },
        {
          question: 'Can I make cash payments?',
          answer: 'For our recent trip to S.A. I booked several accommodation thru SA Places. I just wanted to tell you that everything worked out perfectly with all the bookings and also your booking was very quick and professional. I hope I have the opportunity to re-visit South Africa soon, I will then make my bookings with your company again. I will also recommend',
          expand: false
        },
        {
          question: 'How do I get the payment complete?',
          answer: 'For our recent trip to S.A. I booked several accommodation thru SA Places. I just wanted to tell you that everything worked out perfectly with all the bookings and also your booking was very quick and professional. I hope I have the opportunity to re-visit South Africa soon, I will then make my bookings with your company again. I will also recommend',
          expand: false
        }
      ]
    }
  },
  methods: {
    itemCollapse(index) {
        this.questionsAndAnswersList = this.questionsAndAnswersList.map((item, i) => {
            item.expand = !item.expand
            if (i !== index) {
                item.expand = false 
            }
            return item;
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
    margin-bottom: -5px;
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

.nav-link-question {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 500;
    font-size: 0.8em;
    line-height: 35px;
    letter-spacing: -0.2px;
    color: #FFFFFF;
    padding-bottom: 10px !important;
}

.nav-link {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: normal;
    font-size: 16px;
    line-height: 30px;
    color: #FFFFFF;
    text-decoration: none;
    padding-left: 0px;
    padding-right: 0px;
    padding-bottom: 30px;
}

.nav-link.answer {
    opacity: 0.7;
}

.nav-link.answer:hover {
    color: #FFFFFF !important;
    opacity: 0.7;
}

.arrow {
    border-style: solid;
    border-width: 0 3px 3px 0;
    border-image: linear-gradient(180deg, #9672FF 0%, #6B4FE8 100%) 1;
    float: right;
    padding: 3px;
    margin-right: 20px;
    margin-top: 0.8em;
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