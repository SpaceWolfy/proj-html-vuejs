<template>
  <div>
    <div class="main">
      <div class="text">
        <div class="title">Contact with our team</div>
        <p>If you are planning on developing a product landing.</p>
      </div>

      <div class="contact-info">
        <div class="left-side">
          <div class="map">
            <img src="../../assets/img/StaticMapService.GetMapIma.png" alt="" />

            <div class="indicazioni">
              <div class="left-part">
                <div>Storey Ave</div>
                <div>San Francisco, California 94129</div>
                <div>Visualizza mappa più grande</div>
              </div>
              <div class="right-part">
                <img src="../../assets/img/indicazioni.png" alt="" />
                <div>Indicazi...</div>
              </div>
            </div>

            <div class="zoom">
              <i class="fas fa-plus"></i>
              <div class="line"></div>
              <i class="fas fa-minus"></i>
            </div>

            <div class="location">
              <img src="../../assets/img/pointmap.png" alt="" />
            </div>

            <div class="legal-info">
              <div>Dati mappa ©2020</div>
              <div>Termini e condizioni d'uso</div>
              <div>Segnala un errore nella mappa</div>
            </div>
          </div>
        </div>

        <div class="right-side">
          <img class="logo" src="" alt="" />

          <div class="street"></div>

          <div class="contacts">
            <div></div>
            <div></div>
          </div>

          <div class="social"></div>

          <div class="input-section">
            <div class="subtitle"></div>

            <div class="personal info"></div>

            <div></div>

            <div class="user-message"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "@/style/Variables.scss";

.main {
  margin: 110px 135px 0 135px;

  .text {
    text-align: center;
    margin-bottom: 110px;
    .title {
      font-size: 38px;
      margin-bottom: 20px;
    }

    p {
      font-size: 17px;
      line-height: 30px;
    }
  }

  .contact-info {
    .left-side {
      .map {
        position: relative;
        width: 555px;
        height: 450px;

        .indicazioni,
        .zoom,
        .location,
        .legal-info {
          position: absolute;
        }

        .indicazioni {
          background-color: white;
          top: 10px;
          left: 10px;
          padding: 10px;
          display: flex;
          cursor: pointer;

          .left-part {
            div:first-child {
              color: $darkGrey;
              font-weight: 600;
              font-size: 14px;
            }

            div:nth-child(2),
            div:last-child {
              font-weight: bold;
              font-size: 12px;
            }

            div:nth-child(2) {
              color: #7e7e7e;
              margin: 5px 0 22px 0;
            }

            div:last-child {
              color: $blue;
            }
          }

          .right-part {
            text-align: center;
            margin: 0 20px 0 40px;
            img {
              width: 21px;
            }

            div {
              color: $blue;
              font-size: 12px;
            }
          }
        }

        .zoom {
          display: flex;
          flex-direction: column;
          background-color: white;
          color: #666666;
          right: 10px;
          bottom: 30px;
          border: 1px solid #e6e6e6;
          cursor: pointer;

          .line {
            border-top: 1px solid #e6e6e6;
            margin: 0 5px;
          }

          i {
            padding: 10px;
            font-size: 23px;
          }
        }

        .location {
          top: 205px;
          left: 50%;
          transform: translate(-50%, -50%);
        }

        .legal-info {
          display: flex;
          color: #262826;
          font-size: 11px;
          font-weight: bold;
          bottom: 0;
          right: 0;

          div {
            background-color: rgba($color: #e6f1e6, $alpha: 0.8);
            padding: 2px 8px;
            margin-left: 2px;
            cursor: pointer;
          }
        }
      }
    }
  }
}
</style>
