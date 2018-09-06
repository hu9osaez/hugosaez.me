<template>
  <div class="home">
    <header>
      <div class="avatar">
        <img :src="require('@/assets/img/avatar.png')">
      </div>
      <div class="content">
        <h1>Hugo<strong>Sáez</strong></h1>
        <p>
          Full-Stack Developer &bull;
          <span class="heart">❤</span> for servers
        </p>
        <ul class="social">
          <li>
            <a href="https://github.com/hu9osaez" target="_blank"><i class="icon-github"></i></a>
          </li>
          <li>
            <a href="https://twitter.com/hu9osaez" target="_blank"><i class="icon-twitter"></i></a>
          </li>
        </ul>
      </div>
    </header>
    <footer>
      <div class="location">
        <i class="icon-marker"></i>
        <span>Santiago, Chile</span>
      </div>

      <ul>
        <li>
          <a href="mailto:hello@hugosaez.me">
            <i class="icon-mail"></i>
          </a>
        </li>
        <li>
          <a href="/resume.pdf" target="_blank">Resume</a>
        </li>
      </ul>
    </footer>
  </div>
</template>

<style lang="scss" scoped>
@import '~@/assets/sass/_variables';

header {
  display: flex;
  @include bp('xs') {
    flex-direction: column;
    align-items: center;
  }
  .avatar img {
    max-width: 9rem;
    border-radius: 50%;
    float: left;
    margin-right: 30px;
    border: 7px solid $secondary-color;
    @include bp('xs') {
      margin-right: 0;
      max-width: 8rem;
      float: none;
    }
  }
  .content {
    display: block;
    @include bp('xs') {
      text-align: center;
    }
    h1 {
      font-family: 'Roboto', sans-serif;
      font-size: 2rem;
      text-transform: uppercase;
      letter-spacing: -2px;
      margin-top: 7px;
      strong {
        letter-spacing: 1px;
        margin-left: 2px;
      }
    }
    p {
      color: grey;
      margin-left: 2px;
      margin-top: 5px;
      .heart {
        color: #B71C1C;
        font-size: 16px;
      }
    }
    .social {
      margin-left: 2px;
      margin-top: 8px;
      li {
        display: inline-block;
        a {
          color: #545454;
          height: 30px;
          padding: 5px 3px;
          i {
            font-size: 1.5rem;
          }
        }
      }
    }
  }
}
footer {
  align-self: flex-end;
  display: flex;
  justify-content: space-between;
  margin-top: 25px;
  text-transform: uppercase;
  width: 100%;
  @include bp('xs') {
    align-items: center;
    flex-direction: column;
    margin-top: 15px;
  }
  .location {
    display: block;
    padding: 4px 5px 3px;
    height: 24px;
    @include bp('xs') {
      margin-bottom: 15px;
    }
    i {
      color: #545454;
      margin-right: 5px;
    }
    span {
      font-size: .8rem;
      line-height: 20px;
    }
  }
  ul li {
    display: inline-block;
    margin: 0 5px 0 0;
    padding: 0;
    &:last-child { margin-right: 0 }
    a {
      border: 1px solid #d0d0d0;
      border-radius: 3px;
      color: #545454;
      display: inline-block;
      height: 24px;
      padding: 4px 5px 3px;
      transition: all 400ms;
      &:hover { border-color: #bdbdbd }
    }
  }
}
</style>

