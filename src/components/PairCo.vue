<template>
  <div class="container">
    <div class="section-1">
      <div class="left-content">
        <div class="logo">
          <img src="../assets/LOGO_PAIR-CO_PNG-02 1.svg" alt="" />
        </div>
        <div class="content">
          <div id="sec1-head1" class="heading">{{ section_1_heading_1 }}</div>
          <div id="sec1-head2" class="heading">{{ section_1_heading_2 }}</div>
          <div id="sec1-detail" class="description">
            {{ section_1_head_description }}
          </div>
          <button id="sec1-btn" class="all-course">{{ all_course }}</button>
        </div>
      </div>
      <div class="section1-right-img">
        <img
          id="sec1-img"
          src="../assets/intro.png"
        />
      </div>
    </div>
    <div class="section-2">
      <div class="section2-left">
        <img id="sec2-img" src="../assets/section-2.svg" alt="" />
      </div>
      <div class="content">
        <div class="heading">
          <span id="sec2-head1">{{ section_2_heading_1 }}</span>
          <span id="sec2-head2">{{ section_2_heading_2 }}</span>
        </div>
        <div id="sec2-sub-head" class="sub-heading">{{ section_2_sub_heading }}</div>
        <div id="sec2-description" class="description">{{ section_2_description }}</div>
        <button id="sec2-btn" class="find-course">{{ find_course }}</button>
      </div>
    </div>
    <div class="section-3">
      <div id="sec3-keyword" class="keyword">{{ section_3_word }}</div>
      <button id="sec3-btn" class="all-course">{{ all_course }}</button>
    </div>
    <div class="section-4">
      <div class="one-plus-one">
        <span id="sec4-f1" class="first-one">{{ section_4_first_one }}</span>
        <span id="sec4-s1" class="second-one">{{ section_4_second_one }}</span>
      </div>
      <div id="sec4-word" class="word">{{ section_4_word }}</div>
    </div>
    <div class="section-5">
      <div>{{ section_5_word1 }}</div>
      <div>{{ section_5_word2 }}</div>
    </div>
    <div class="section-6">
      <div class="head">
        <div class="heading">
          <span id="sec6-word1">{{ section_6_word1 }}</span>
          <span id="sec6-word2">{{ section_6_word2 }}</span>
        </div>
        <div class="see-all">
          {{ section_6_see_all }}
        </div>
      </div>
      <div class="grid"></div>
    </div>
    <div class="section-7">
      <div id="sec7-heading">{{ section_7_heading }}</div>
      <div id="sec7-sub-heading">{{ section_7_sub_heading }}</div>
    </div>
    <div class="section-8">
      <div id="sec8-heading">{{ section_8_partner }}</div>
      <div class="partners">
        <div class="partner">
          <img src="../assets/odds.png" alt="">
        </div>
        <div class="partner">
          <img src="../assets/artisan.png" alt="">
        </div>
        <div class="partner">
          <img src="../assets/camt.png" alt="">
        </div>
      </div>
    </div>
    <div class="section-9"></div>
  </div>
</template>

<script>
import { gsap } from "gsap";
import { ScrollTrigger } from "gsap/ScrollTrigger";
import ScrollMagic from "scrollmagic";

var controller = new ScrollMagic.Controller();

gsap.registerPlugin(ScrollTrigger);
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  data() {
    return {
      section_1_heading_1: "เราพร้อม",
      section_1_heading_2: "ติดอาวุธให้องค์กรของคุณ",
      section_1_head_description:
        "ด้วยเทคโนโลยีที่คัดสรรมาอย่างดี รวมเป็นคอร์สที่น่าสนใจ เพื่อช่วยยกระดับองค์กรของคุณ",
      all_course: "ดูคอร์สทั้งหมด",
      section_2_heading_1: "ลดเวลา ",
      section_2_heading_2: "ลดค่าใช้จ่าย",
      section_2_sub_heading: "ด้วย Serverless Course",
      section_2_description:
        "สร้าง application โดยไม่ใช้ server หรือ back-end ใดๆ ซึ่งช่วยประหยัดเวลาในการทำงาน และลดค่าใช้จ่ายในการดำเนินงาน",
      find_course: "ดูรายละเอียดเพิ่มเติม",
      section_3_word: "ถ้าคุณยังไม่จุใจ เรายังมีคอร์สอีกมากมายให้คุณได้ค้นหา",
      section_4_first_one: "1",
      section_4_second_one: "+1",
      section_4_word: "เป็นได้มากกว่าสอง",
      section_5_word1: "ที่แพร์-โค",
      section_5_word2: "เราเชื่อมั่นว่า “การร่วมมือกันจะนำไปสู่ศักยภาพที่มากกว่า”",
      section_6_word1: "เล่นเล็กก็ได้",
      section_6_word2: "เล่นใหญ่ก็เคย",
      section_6_see_all: "ดูทั้งหมด",
      section_7_heading: "PAIR-CO LABO",
      section_7_sub_heading: "เรียนรู้ไปพร้อมกับเรา",
      section_8_partner: "Our Partner"
    };
  },
  mounted() {
    const tl_logo = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    const tl_sec1_h1 = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    const tl_sec1_h2 = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    const tl_sec1_detail = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    const tl_sec1_btn = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    const tl_sec2_img = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    const tl_sec2_head1 = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    const tl_sec2_head2 = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    const tl_sec2_sub_head = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    const tl_sec2_description = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    const tl_sec2_btn = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    const tl_sec3_keyword = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    const tl_sec3_btn = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    const tl_sec4_f1 = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    const tl_sec4_word = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    const tl_sec6_word1 = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    const tl_sec6_word2 = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    const tl_sec7_heading = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    const tl_sec7_sub_head = gsap.timeline({
      scrollTrigger: {
        trigger: ".trigger",
        scrub: true,
      },
    });
    tl_logo.to(".logo", { x: -650, y: -450, duration: 1, scale: 0.5 });
    tl_sec1_h1.to("#sec1-head1", { delay: 0, opacity: 1, duration: 1 });
    tl_sec1_h2.to("#sec1-head2", { delay: 0.1, opacity: 1, duration: 2 });
    tl_sec1_detail.to("#sec1-detail", { delay: 0.2, opacity: 1, duration: 1 });
    tl_sec1_btn.to("#sec1-btn", { delay: 0.3, opacity: 1, duration: 1 });
    tl_sec2_img.to("#sec2-img", { delay: 0.4, y: -40, opacity: 1, duration: 1 });
    tl_sec2_head1.to("#sec2-head1", { delay: 0.4, opacity: 1, duration: 1 });
    tl_sec2_head2.to("#sec2-head2", { delay: 0.5, opacity: 1, duration: 1 });
    tl_sec2_sub_head.to("#sec2-sub-head", { delay: 0.55, opacity: 1, duration: 1 });
    tl_sec2_description.to("#sec2-description", { delay: 0.6, opacity: 1, duration: 1 });
    tl_sec2_btn.to("#sec2-btn", { delay: 0.7, opacity: 1, duration: 1 });
    tl_sec3_keyword.to("#sec3-keyword", { delay: 1, opacity: 1, duration: 1 });
    tl_sec3_btn.to("#sec3-btn", { delay: 1.1, opacity: 1, duration: 1 });
    tl_sec4_f1.to("#sec4-f1", { delay: 1.2, opacity: 1, duration: 1 });
    tl_sec4_word.to("#sec4-word", { delay: 1.3, opacity: 1, duration: 1 });
    tl_sec6_word1.to("#sec6-word1", { delay: 3, opacity: 1, duration: 1 });
    tl_sec6_word2.to("#sec6-word2", { delay: 3.2, opacity: 1, duration: 1, fontSize: "3.2rem" });
    tl_sec7_heading.to("#sec7-heading", { delay: 3, opacity: 1, duration: 1 });
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container {
  background-image: url("../assets/intro_bg.svg");
  background-size: 100% auto;
  background-repeat: no-repeat;
  padding: 0 40px;
  padding-top: 40px;
  .section-1 {
    padding: 0 80px;
    padding-top: 40px;
    padding-bottom: 280px;
    display: flex;
    .left-content {
      flex:1.5;
      display: flex;
      flex-direction: column;
      margin-top: 120px;
      .content {
        color: #fff;
        .heading {
          font-size: 4.8rem;
          line-height: 125%;
          opacity: 0;
        }
        .description {
          margin-top: 32px;
          font-size: 1.2rem;
          opacity: 0;
        }
      }
    }
    .section1-right-img {
      flex: 1;
      #sec1-img {
        width: 100%;
        height: auto;
      }
    }
  }
  .section-2 {
    display: flex;
    margin: 0 80px;
    margin-top: 64px;
    .section2-left {
      flex: 1;
      img {
        width: 100%;
        height: auto;
        opacity: 0;
      }
    }
    .content {
      flex: 1;
      margin-top: 20px;
      padding-left: 40px;
      .heading {
        font-size: 4rem;
        line-height: 100%;
        color: #0072bb;
      }
      #sec2-head1 {
        opacity: 0;
      }
      #sec2-head2 {
        opacity: 0;
      }
      .sub-heading {
        font-size: 2.5rem;
        line-height: 100%;
        color: #48b6cc;
        opacity: 0;
      }
      .description {
        margin-top: 32px;
        margin-bottom: 72px;
        color: #686868;
        opacity: 0;
      }
      .find-course {
        font-family: Supermarket;
        font-size: 1.2rem;
        color: #fff;
        background: #0072bb;
        padding: 4px 16px;
        border: none;
        border-radius: 50px;
        opacity: 0;
      }
    }
  }
  .section-3 {
    text-align: center;
    padding: 300px 0;
    background-image: url("../assets/section-3.png");
    width: 100%;
    height: 100%;
    .keyword {
      color: #fff;
      font-size: 2.5rem;
      opacity: 0;
    }
  }
}
.section-4 {
  padding: 50px 0;
  .one-plus-one {
    font-family: Kanit;
    font-size: 16rem;
    background: -webkit-linear-gradient(#70dccf, #0072bb);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    text-align: center;
    .first-one {
      opacity: 0;
    }
    .second-one {
      
    }
  }
  .word {
    text-align: center;
    color: #888888;
    font-size: 2.5rem;
    opacity: 0;
  }
}
.section-5 {
}
.section-6 {
  padding: 0 80px;
  .head {
    display: flex;
    .heading {
      #sec6-word1 {
        font-size: 2.5rem;
        color: #686868;
        opacity: 0;
      }
      #sec6-word2 {
        font-size: 2.5rem;
        color: #0072bb;
        opacity: 0;
      }
    }
  }
}
.section-7 {
  padding: 0 80px;
  align-items: center;
  display: flex;
  flex-direction: column;
  #sec7-heading {
    font-size: 4.8rem;
    font-family: Arabica;
    color: #0072BB;
    text-shadow: -2px 2px #FEC449;
    opacity: 0;
  }
  #sec7-sub-heading {
    font-size: 2.5rem;
    color: #686868;
    opacity: 0;
  }
}
.section-8 {
  display: flex;
  flex-direction: column;
  #sec8-heading {
    text-align: center;
    font-size: 2.2rem;
    color: #686868;
  }
  .partners {
    display: flex;
    margin: 120px;
    justify-content: center;
    align-items: center;
    .partner {
      flex: 1;
      justify-content: center;
    }
  }
}
.all-course {
  font-family: Supermarket;
  font-size: 1.2rem;
  color: #0072bb;
  background: #ffffff;
  padding: 4px 16px;
  border: none;
  border-radius: 50px;
  margin-top: 48px;
  opacity: 0;
}
</style>
