<template>
  <main>
    <section class="first-section">
      <div class="container">
        <div class="row">
          <div class="col d-flex justify-content-center">
            <div class="mybox p-4">
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
            <div class="mybox p-4 me-4 ms-4">
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
            <div class="mybox p-4">
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
      .icons {
        width: 50px;
        height: 50px;
        border-radius: 50%;
        background-color: #DAECED;
        span {
          color: #1a948f;
          display: inline-block;
          transform: translate(30%, 20%);
          font-size: 1.5em;
        }
      }
    }
  }
</style>