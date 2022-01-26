<template>
  <footer>
    <div class="footer-top">
      <div class="container">
        <div class="row">
          <div class="col-8">
            <div class="text">
              <span class="subtitle">
                send a message
              </span>
              <div class="title">
                <span class="color-title">
                  Get in
                </span>
                <span class="bg-title">
                  Touch
                </span>
              </div>
              <p>
                We will respond to your message as soon as possible.
              </p>
            </div>
            <form class="row g-3">
              <div class="col-md-6">
                <input type="name" placeholder="Name" class="form-control" id="inputName">
              </div>
              <div class="col-md-6">
                <input type="email" placeholder="Email" class="form-control" id="inputMail">
              </div>
              <div class="col-md-6">
                <input type="text" placeholder="Phone" class="form-control" id="inputPhone">
              </div>
              <div class="col-md-6">
              <select class="form-select" aria-label="Default select example">
                <option selected > More info</option>
                <option value="1">One</option>
                <option value="2">Two</option>
                <option value="3">Three</option>
              </select>
              </div>
              <div class="mb-3">
                <textarea class="form-control" placeholder="Message" id="exampleFormControlTextarea1" rows="3"></textarea>
              </div>
              <div class="col-12">
                <button type="submit" class="btn btn-form">send</button>
              </div>
            </form>
          </div>
          <div class="col-4">
            <h3>
              Example Inc.
            </h3>
            <p v-for="(text, index) in texts" :key="index">
              {{text.paragraph}}
            </p>
            <ul>
              <li v-for="(contact, index) in contacts" :key="index">
                <a :href="contact.href">
                  <span class="round-icon">
                    <i :class="contact.icon"></i>
                  </span>
                  <span>
                    {{contact.text}}
                  </span>
                </a>
              </li>
            </ul>
            <button type="button" class="btn read ms-2">view map</button>
          </div>
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <div class="container">
        <div class="row pt-3 pb-3">
          <div class="col d-flex justify-content-between">
            <div class="container-left">
              <span>
                &copy; 2021 NEXGEN is Proudly Powered by Codings.
              </span>
            </div>
            <div class="container-right">
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
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  data() {
    return {
      contacts: [
        {
          icon: 'fas fa-phone-alt',
          text: '+1(305) 1234-5678',
          href: '#'
        },
        {
          icon: 'fas fa-envelope',
          text: 'hello@example.com',
          href: '#'
        },
        {
          icon: 'fas fa-map-marker-alt',
          text: 'Main Avenue, 987',
          href: '#'
        },
      ],
      texts: [
        {
          paragraph: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.'
        },
        {
          paragraph: 'Praesent diam lacus dapibus sed imperdiet consecteur.'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
/* @import "../assets/scss/style.scss"; */
  footer {
    .footer-top {
      background-color: #111117;
      padding: 100px 0 ;
      .text {
        padding-bottom: 20px;
        .subtitle {
          text-transform: uppercase;
          color: #1a948f;
          font-weight: 700;
          font-size: 1.3em; 
          display: inline-block;
          margin-bottom: 20px;
        }
        .title {
          .bg-title {
            color: #ffffff;
            background-color: #0E272D;
            border-radius: 5px;
            padding: 0 15px;
            display: inline-block;
            font-size: 2.5em;
            font-weight: bold;
          }
          .color-title {
            font-size: 2.5em;
            font-weight: bold;
            color: #ffffff;
          }
        }
        p {
          color: #797D83;
          margin: 20px 0;
          font-size: 1.2em;
        }
      }
      form {
        input, select, textarea {
          background-color: #1D1D23;
          border: none;
          color: #777777;
        }
        .btn-form {
          padding: 5px 20px;
          background-color: #1a948f;
          color: #ffffff;
          text-transform: uppercase;
        }
      }
      h3 {
        color: #ffffff;
        font-weight: bold;
      }
      p {
        color: #797D83;
        width: 300px;
      }
      ul {
        list-style-type: none;
        padding: 0;
        li {
          margin-bottom: 15px;
          a {
            text-decoration: none;
            color: #1a948f;
            display: flex;
            align-items: center;
            margin-left: 5px;
            .round-icon {
              background-color: #0F2128;
              width: 40px;
              height: 40px;
              border-radius: 50%;
              display: flex;
              align-items: center;
              justify-content: center;
              margin-right: 10px;
            }
          }
        }
      }
      .read {
        text-transform: uppercase;
        background-color: transparent;
        padding: 5px 20px;
        color: white;
        border: 1px solid #1a948f;
      }
    }
    .footer-bottom {
      background-color: #16161C;
      color: #777777;
      .container-left {
        cursor: pointer;
      }
      .container-left:hover {
        color: #1a948f;
      }
      .container-right {
        cursor: pointer;
      }
      span:hover {
        color: #1a948f;
      }
    }
  }
</style>