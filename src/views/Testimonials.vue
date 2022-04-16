<template>

  <div class="container testimonials grid">
    <TestimonialCard :testimonials="testimonials" />
  </div>
</template>

<script>
  import TestimonialCard from '@/components/TestimonialsCard.vue'
  //import dataTestimonials from '@/data/testimonials.js'
export default {
  data() {
    return {
      testimonials: [
        {
          img: "https://images.unsplash.com/photo-1509967419530-da38b4704bc6?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=895&q=80",
          name: "Veronica Ribeiro",
          profession: "UX/UI Designer",
          title:
            "This challenge will be perfect practice for anyone wanting to test their CSS Grid skills. Grid is such a powerful addition to CSS, soit's worth getting to grips with it!",
          description:
            "Your challenge is to build out this testimonials grid section and get it looking as close to the design as possible. You can use any tools you like to help you complete the challenge.",
          tag: "primary",
        },

        {
          img: "https://images.unsplash.com/photo-1509967419530-da38b4704bc6?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=895&q=80",
          name: "André Júnior",
          profession: "Backend",
          title:
            "This challenge will be perfect practice for anyone wanting to testtheir CSS Grid skills.",
          description:
            "Your challenge is to build out this testimonials grid section and get it looking as close to as possible.",
          tag: "tertiary",
        },
        {
          img: "https://images.unsplash.com/photo-1509967419530-da38b4704bc6?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=895&q=80",
          name: "Elton Andrade",
          profession: "CEO",
          title:
            "This challenge will be perfect practice for anyone wanting to testtheir CSS Grid skills.",
          description:
            "Your challenge is to build out this testimonials grid section and get it looking as close to the design as possible. You can use any tools you like to help you complete the challenge. So if you've got something you'd like to practice, feel free to give it a go. Your challenge is to build out this testimonials grid section and get it looking as close to the design as possible. You can use any tools you like to help you complete the challenge. So if you've got something you'd like to practice, feel free to give it a go.",
          tag: "",
        },
        {
          img: "https://images.unsplash.com/photo-1509967419530-da38b4704bc6?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=895&q=80",
          name: "Rafaela Ventura",
          profession: "QA",
          title:
            "This challenge will be perfect practice for anyone wanting to testtheir CSS Grid skills.",
          description:
            "Your challenge is to build out this testimonials grid section and get it looking as close to as possible.",
          tag: "",
        },
        {
          img: "https://images.unsplash.com/photo-1509967419530-da38b4704bc6?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=895&q=80",
          name: "Beatriz Rodrigues",
          profession: "Agile",
          title:
            "This challenge will be perfect practice for anyone wanting to testtheir CSS Grid skills.",
          description:
            " Your challenge is to build out this testimonials grid section and get it looking as close to the design as possible. You can use any tools you like to help you complete the challenge. So if you've got something you'd like to practice, feel free to give it a go.",
          tag: "secondary",
        },
      ],
    };
  },
  components:{
      TestimonialCard
  }
};
</script>

<style lang="scss">
@import "@/style/color.scss";

.testimonials {
  grid-template-columns: repeat(4, 1fr);
  gap: 16px;
}
.testimonial:nth-child(3) {
  grid-row: span 2;
}
.testimonial:nth-child(1) {
  grid-column: span 2;
}
.testimonial:nth-child(5) {
  grid-column: span 2;
}

.testimonial {
  background-color: $White;

  padding: 16px;
  border-radius: 8px;
  color: $Fiord;
  box-shadow: 1px 1px 8px #ababac;
  height: 100%;
  h2 {
    font-size: 18px;
    font-weight: 800;
    line-height: normal;
    margin: 8px 0;
  }
  h3 {
    line-height: 1;
  }
  .name {
    margin-left: 8px;
  }
  span {
    font-size: 10px;
    margin: 0;
    padding: 0;
    line-height: 1;
    text-transform: uppercase;
  }

  &.primary {
    background-color: $PurpleHeart;
    color: $White;
  }
  &.secondary {
    background-color: $Mirage;
    color: $White;
  }
  &.tertiary {
    background-color: $Fiord;
    color: $White;
  }
  .testimonial_user {
    display: flex;
    img {
      width: 50px;
      height: 50px;
      border-radius: 50%;
      object-fit: cover;
    }
  }
}
@media only screen and (max-width: 1024px) {
  .testimonials {
    grid-template-columns: 1fr;
    gap: 16px;
  }
  .testimonial{
      grid-column: span 2;
  }
  
}

</style>
