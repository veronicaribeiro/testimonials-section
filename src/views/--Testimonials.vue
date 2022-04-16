<template>
  <div class="container testimonials flex gap16">
    <div class="flex flex3 gap16 column justify-c-space-between">
      <div class="flex align-item-stretch gap16">
        <div class="testimonial primary flex2">
          <div class="testimonial_user">
            <img
              src="https://images.unsplash.com/photo-1509967419530-da38b4704bc6?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=895&q=80"
              alt=""
            />
            <div class="name">
              <h3 class="name">Veronica</h3>
              <span class="status">UX/UI Designer</span>
            </div>
          </div>
          <div class="testimonial-container">
            <h2>
              This challenge will be perfect practice for anyone wanting to test
              their CSS Grid skills. Grid is such a powerful addition to CSS, so
              it's worth getting to grips with it!
            </h2>
            <p>
              Your challenge is to build out this testimonials grid section and
              get it looking as close to the design as possible. You can use any
              tools you like to help you complete the challenge.
            </p>
          </div>
        </div>

        <div class="testimonial tertiary flex1">
          <div class="testimonial_user">
            <img
              src="https://images.unsplash.com/photo-1509967419530-da38b4704bc6?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=895&q=80"
              alt=""
            />
            <div class="name">
              <h3>Veronica</h3>
              <span class="status">UX/UI Designer</span>
            </div>
          </div>
          <div class="testimonial-container">
            <h2>
              This challenge will be perfect practice for anyone wanting to test
              their CSS Grid skills.
            </h2>
            <p>
              Your challenge is to build out this testimonials grid section and
              get it looking as close to as possible.
            </p>
          </div>
        </div>
      </div>
      <div class="flex align-item-stretch gap16">
        <div class="testimonial flex1">
          <div class="testimonial_user">
            <img
              src="https://images.unsplash.com/photo-1509967419530-da38b4704bc6?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=895&q=80"
              alt=""
            />
            <div class="name">
              <h3>Veronica</h3>
              <span class="status">UX/UI Designer</span>
            </div>
          </div>
          <div class="testimonial-container">
            <h2>
              This challenge will be perfect practice for anyone wanting to test
              their CSS Grid skills.
            </h2>
            <p>
              Your challenge is to build out this testimonials grid section and
              get it looking as close to the possible.
            </p>
          </div>
        </div>

        <div class="testimonial secondary flex2">
          <div class="testimonial_user">
            <img
              src="https://images.unsplash.com/photo-1509967419530-da38b4704bc6?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=895&q=80"
              alt=""
            />
            <div class="name">
              <h3>Veronica</h3>
              <span class="status">UX/UI Designer</span>
            </div>
          </div>
          <div class="testimonial-container">
            <h2>
              This challenge will be perfect practice for anyone wanting to test
              their CSS Grid skills. Grid is such a powerful addition to CSS, so
              it's worth getting to grips with it!
            </h2>
            <p>
              Your challenge is to build out this testimonials grid section and
              get it looking as close to the design as possible. You can use any
              tools you like to help you complete the challenge. So if you've
              got something you'd like to practice, feel free to give it a go.
            </p>
          </div>
        </div>
      </div>
    </div>
    <div class="flex1 coluna2">
      <div class="testimonial">
        <div class="testimonial_user">
          <img
            src="https://images.unsplash.com/photo-1509967419530-da38b4704bc6?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=895&q=80"
            alt=""
          />
          <div class="name">
            <h3>Veronica</h3>
            <span class="status">UX/UI Designer</span>
          </div>
        </div>
        <div class="testimonial-container">
          <h2>
            This challenge will be perfect practice for anyone wanting to test
            their CSS Grid skills. Grid is such a powerful addition to CSS, so
            it's worth getting to grips with it!
          </h2>
          <p>
            Your challenge is to build out this testimonials grid section and
            get it looking as close to the design as possible. You can use any
            tools you like to help you complete the challenge. So if you've got
            something you'd like to practice, feel free to give it a go.
          </p>

          <p>
            Your challenge is to build out this testimonials grid section and
            get it looking as close to the design as possible.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
@import "@/style/color.scss";
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
</style>
