<template>
  <div class="header-container">
    <div class="header">
      <div class="container">
        <div class="row pt-3 pb-3">
          <div class="col d-flex justify-content-between">
            <div class="left">
              <span>
                <i class="fas fa-clock"></i>
              </span>
              <span class="ms-2">Open Hours: Mon - Sat - 9:00 - 18:00</span>
            </div>
            <div class="right">
              <span>
                <i class="fas fa-phone-alt"></i>
              </span>
              <span class="ms-2 me-4">+1 (305) 1234-5678</span>
              <span>
                <i class="fas fa-envelope"></i>
              </span>
              <span class="ms-2 me-4">hello@example.com</span>
              <span>
                <i class="fab fa-facebook-f"></i>
              </span>
              <span class="ms-4 me-4">
                <i class="fab fa-twitter"></i>
              </span>
              <span>
                <i class="fab fa-linkedin-in"></i>
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="jumbotron">
      <div class="bg-opacity">
          <div class="container">
            <div class="row">
              <div class="col pt-4 d-flex justify-content-between">
                <div class="jumbo-left">
                  <span class="next">
                    n e x
                  </span>
                  <span class="gen">
                    g e n
                  </span> 
                </div>
                <div class="jumbo-right">
                  <div>
                    <a v-for="(link, index) in links" :key="index" :href="link.href">{{link.namelink}}</a>
                    <a href="#"> <i class="far fa-user"></i> </a>
                    <button type="button" class="btn">get in touch</button>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="jumbo-text">
            <div class="container">
              <div class="row">
                <div class="col-6">
                  <span class="subtitle">
                    human resources
                  </span>
                  <h1 class="title-bg">
                    Get More
                  </h1>
                  <div class="container-bg mb-4">
                    <div class="bg-h1">
                    </div>
                    <div class="container-title">
                      <h1 class="title-bg">Productivity</h1>
                    </div>
                  </div>
                  <p class="mb-4">Planning, recruitment and selection process and performance evaluation of employees.</p>
                  <button type="button" class="btn">get in touch</button>
                  <button type="button" class="btn read ms-2">read more</button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      links: [
        {
          namelink: 'home',
          href: '#'
        },
        {
          namelink: 'about',
          href: '#'
        },
        {
          namelink: 'projects',
          href: '#'
        },
        {
          namelink: 'process',
          href: '#'
        },
        {
          namelink: 'testimonials',
          href: '#'
        },
      ]
    }
  }
}
</script>

<style lang="scss">
// @import "../assets/scss/style.scss";
  .header {
    background-color: #24343c;
    .container {
      .row {
        .col {
          span {
            color: #babdbe;
          }
          .left:hover span {
            color: #1a948f;
            cursor: pointer;
          }
          span:hover {
            color: #1a948f;
            cursor: pointer;
          }
        }
      }
    }
  }
  .jumbotron {
    background-image: url('../assets/img/bg-4.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    .bg-opacity {
      width: 100%;
      height: 100%;
      background-color: rgba(0, 0, 0, 0.5);
      .container {
        .row {
          .col {
            .jumbo-left {
              span {
                text-transform: uppercase;
                font-weight: bold;
                font-size: 1.3em;
              }
              .next {
                color: #00A6A6;
                background-color: #1D3B3A;
                border-top-left-radius: 25px;
                border-bottom-left-radius: 25px;
                padding: 10px 0 10px 30px;
                margin-right: 2px;
              }
              .gen {
                color: #babdbe;
              }
            }
            .jumbo-right {
              a {
                margin-right: 30px;
                text-transform: uppercase;
                text-decoration: none;
                font-weight: 600;
                color: white;
              }
              button {
                text-transform: uppercase;
                padding: 8px 30px;
                background-color: #1a948f;
                color: #ffffff;
              }
              a:hover {
                color: #1a948f;
              }
              .btn {
                margin-right: 0;
              }
            }
          }
        }
      }
    }
    .jumbo-text {
      padding: 170px 0 630px 0;
      .subtitle {
        text-transform: uppercase;
        color: #1a948f;
        font-weight: 700;
        font-size: 1.3em; 
      }
      .title-bg {
        font-size: 3.7em;
        font-weight: bold;
        color: #ffffff;
        position: relative;
        z-index: 999;
      }
      .container-bg {
        position: relative;
        height: 65px;
        width: 345px;
        .bg-h1 {
          background-color: #1a948f;
          height: 30px;
          width: 345px;
          position: absolute;
          bottom: 0;
        }
        .container-title {
          .title-bg {
            font-size: 3.7em;
            font-weight: bold;
            color: #ffffff;
          }
        }
      }
      p {
        font-size: 1.5em;
        color: #babdbe;
      }
      button {
        text-transform: uppercase;
        padding: 8px 30px;
        background-color: #1a948f;
        color: #ffffff;
      }
      .read {
        background-color: transparent;
        color: white;
        border: 1px solid #1a948f;
      }
    }
  }
</style>