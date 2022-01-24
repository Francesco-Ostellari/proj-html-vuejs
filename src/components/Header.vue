<template>
  <div class="header-container">
    <div class="header">
      <div class="container">
        <div class="row pt-2 pb-2">
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
      <div class="container">
        <div class="row">
          <div class="col pt-3 d-flex justify-content-between">
            <div class="jumbo-left">
              <span class="next">
                nex
              </span>
              <span>
                gen
              </span> 
            </div>
            <div class="jumbo-right">
              <ul>
                <li>
                  <a href="#">home</a>
                </li>
                <li>
                  <a href="#">about</a>
                </li>
                <li>
                  <a href="#">projects</a>
                </li>
                <li>
                  <a href="#">process</a>
                </li>
                <li>
                  <a href="#">testimonials</a>
                </li>
                <li>
                  <a href="#"> <i class="far fa-user"></i> </a>
                </li>
                <li class="btn">
                  <button type="button" class="btn">get in touch</button>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
  .header {
    background-color: #24343c;
    .container {
      .row {
        .col {
          span {
            color: #babdbe;
          }
        }
      }
    }
  }
  .jumbotron {
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
              background-color: #6c9b9c;
              border-top-left-radius: 25px;
              border-bottom-left-radius: 25px;
              padding: 5px 0 5px 20px;
            }
          }
          .jumbo-right {
            ul {
              list-style: none;
              li {
                display: inline;
                margin-right: 30px;
                a {
                  text-transform: uppercase;
                  text-decoration: none;
                  font-weight: 600;
                  color: black;
                }
                button {
                  text-transform: uppercase;
                  padding: 8px 30px;
                  background-color: #1a948f;
                  color: #ffffff;
                }
              }
              li:hover a {
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
  }
</style>