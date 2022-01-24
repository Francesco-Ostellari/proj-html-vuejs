<template>
  <main>
    <section class="first-section">
      <div class="container">
        <div class="row">
          <div class="col d-flex justify-content-center">
            <div class="mybox px-5">
              <div class="text">
                <div class="icons">
                  <span>
                    <i class="fas fa-user-friends"></i>
                  </span>
                </div>
                <div class="container-text-first-section">
                  <h1>
                    Human Capital
                  </h1>
                  <p>
                    Humanizing business Harness the power of technology to improve the way people work.
                  </p>
                </div>
              </div>
            </div>
            <div class="mybox px-5 me-4 ms-4">
              <div class="text">
                <div class="icons">
                  <span>
                    <i class="fas fa-chart-pie"></i>
                  </span>
                </div>
                <div class="container-text-first-section">
                  <h1>
                    Core business
                  </h1>
                  <p>
                    It takes innovative approaches to transform, modernize, and run existing platforms.
                  </p>
                </div>
              </div>
            </div>
            <div class="mybox px-5">
              <div class="text">
                <div class="icons">
                  <span>
                    <i class="fas fa-tachometer-alt"></i>
                  </span>
                </div>
                <div class="container-text-first-section">
                  <h1>
                    Performance
                  </h1>
                  <p>
                    Achieving maximum impact and value from investments in finance and supply chain.
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="second-section">
      <div class="container-fluid">
        <div class="row">
          <div class="col-6">
            <div class="container">
              <div class="row">
                <div class="col">
                  <div class="text">
                    <span class="subtitle">
                      about the network
                    </span>
                    <div class="title">
                      <span class="bg-title">
                        The
                      </span>
                      <span class="color-title">
                        Company
                      </span>
                    </div>
                    <p>
                      Lorem ipsum dolor sit amet consectetur adipisicing elit. Cras iaculis diam varius diam ultreicies lacinia.
                    </p>
                    <div class="container-box d-flex">
                      <div class="box-company">
                        <h1 class="ms-3">
                          0
                        </h1>
                        <div class="title">Employees</div>
                        <div>Lorem ipsum dolor sit amet</div>
                      </div>
                      <div class="box-company me-3 ms-5">
                        <h1 class="ms-3">
                          0
                        </h1>
                        <div class="title">Partners</div>
                        <div>Lorem ipsum dolor sit amet</div>
                      </div>
                      <div class="box-company">
                        <h1 class="ms-3">
                          0
                        </h1>
                        <div class="title">Customers</div>
                        <div>Lorem ipsum dolor sit amet</div>
                      </div>
                    </div>
                    <button type="button" class="btn">get in touch</button>
                    <button type="button" class="btn read ms-2">read more</button>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="col-6">
            <div class="img">
              
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
  .first-section {
    background-color: #e4eae6;
    padding: 100px 0;
    .mybox {
      height: 350px;
      width: 350px;
      background-color: #ffffff;
      border-radius: 10px;
      .text {
        padding: 68px 0;
        .icons {
          width: 50px;
          height: 50px;
          border-radius: 50%;
          background-color: #DAECED;
          margin-bottom: 15px;
          span {
            color: #1a948f;
            display: inline-block;
            transform: translate(30%, 20%);
            font-size: 1.5em;
          }
        }
        .container-text-first-section {
          h1 {
            font-weight: bold;
            color: #24343c;
            margin-bottom: 15px;
            font-size: 2em;
          }
          p {
            color: #797D83;
            font-weight: 400;
            font-size: 1.1em;
          }
        }
      }
    }
  }
  .second-section {
    .text {
      padding: 100px 0;
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
          color: #1a948f;
          background-color: #DAECED;
          border-radius: 5px;
          padding: 0 15px;
          display: inline-block;
          font-size: 2.5em;
          font-weight: bold;
        }
        .color-title {
          font-size: 2.5em;
          font-weight: bold;
          color: #24343c;
        }
      }
      p {
        color: #797D83;
        margin: 20px 0;
      }
      .container-box {
        margin: 40px 0;
        .box-company {
          width: 130px;
          h1 {
            color: #1a948f;
            font-weight: bold;
          }
          .title {
            font-size: 1.7em;
            font-weight: bold;
            color: #24343c;
            margin: 10px 0;
          }
          div {
            color: #797D83;
          }
        }
      }
      button {
        text-transform: uppercase;
        padding: 8px 30px;
        background-color: #1a948f;
        color: #ffffff;
      }
      .read {
        background-color: transparent;
        color: #1a948f;
        border: 1px solid #1a948f;
      }
    }
    .img {
      background-image: url('../assets/img/about-5.jpg');
      background-size: cover;
    }
  }
</style>