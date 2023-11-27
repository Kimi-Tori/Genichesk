<template>
  <section class="home-news mt-6">
    <v-container>
      <div
        class="home-news__block d-flex justify-center flex-column flex-md-row"
      >
        <div class="d-flex mr-md-8">
          <div class="home-news__block-box --big mr-2 mr-md-8">
            <div class="home-news__block-box__item --1">
              <div class="home-news__block-box__item-grayscale pa-5">
                <p class="home-news__block-box__item-title size-parag">
                  Об университете
                </p>
              </div>
            </div>
            <div class="home-news__block-box__item --2 mt-2 mt-md-8">
              <div class="home-news__block-box__item-grayscale pa-5">
                <p
                  class="home-news__block-box__item-title color-white size-parag"
                >
                  Образование
                </p>
              </div>
            </div>
          </div>
          <div class="home-news__block-box --min">
            <div class="home-news__block-box__item --3">
              <div class="home-news__block-box__item-grayscale pa-5">
                <p
                  class="home-news__block-box__item-title color-white size-parag"
                >
                  Наука и<br />инновации
                </p>
              </div>
            </div>
            <div class="home-news__block-box__item --4 mt-2 mt-md-8">
              <div class="home-news__block-box__item-grayscale pa-5">
                <p class="home-news__block-box__item-title size-parag">
                  Приоритет<br />2030
                </p>
              </div>
            </div>
          </div>
        </div>

        <div class="d-flex mt-2 mt-md-0">
          <div class="home-news__block-box --big mr-2 mr-md-8">
            <div class="home-news__block-box__item --5">
              <div class="home-news__block-box__item-grayscale pa-5">
                <p class="home-news__block-box__item-title size-parag">
                  Молодежная<br />политика
                </p>
              </div>
            </div>
            <div class="home-news__block-box__item --6 mt-2 mt-md-8">
              <div class="home-news__block-box__item-grayscale pa-5">
                <p class="home-news__block-box__item-title size-parag">
                  Контакты
                </p>
              </div>
            </div>
          </div>
          <div class="home-news__block-box --min">
            <div class="home-news__block-box__item --7">
              <div class="home-news__block-box__item-grayscale pa-5">
                <p class="home-news__block-box__item-title size-parag">
                  Брендбук
                </p>
              </div>
            </div>
            <div class="home-news__block-box__item --8 mt-2 mt-md-8">
              <div class="home-news__block-box__item-grayscale pa-5">
                <p
                  class="home-news__block-box__item-title color-white size-parag"
                >
                  Приёмная<br />комиссия
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </v-container>
  </section>
</template>

<script>
export default {
  name: "home-news",
  data() {
    return {};
  },
};
</script>

<style lang="scss">
.home-news {
  &__block {
    &-box {
      &.--big {
        width: 100%;

        @include up($md) {
          max-width: 336px;
          min-width: 336px;
        }
      }

      &.--min {
        width: 100%;

        @include up($md) {
          max-width: 192px;
          min-width: 192px;
          width: 100%;
        }
      }

      &__item {
        border-radius: 20px;

        &-title {
          word-wrap: break-word;
          word-break: break-all;
          white-space: normal;

          @include up($md) {
            word-break: normal;
          }
        }

        &-grayscale {
          width: 100%;
          height: 100%;
          border-radius: 20px;
        }

        &.--1 {
          height: 214px;
          background-image: url(@/assets/home/home-news-first.svg);
          background-size: cover;

          &:hover {
            background-image: url(@/assets/home/home-news-first-hover.jpg);
            & > .home-news__block-box__item-grayscale {
              background: $grayscale-gradient;
            }
          }
        }

        &.--2 {
          height: 192px;
          background-color: $main-blue;
          background-image: url(@/assets/home/home-news-two.svg);
          background-position: 105% 105%;

          &:hover {
            background-image: url(@/assets/home/home-news-two-hover.jpg);
            background-size: cover;
            background-position: right;
            & > .home-news__block-box__item-grayscale {
              background: $grayscale-gradient;
            }
          }
        }

        &.--3 {
          height: 164px;
          background: linear-gradient(180deg, $main-blue 0%, $main-blue 100%);
          background-size: cover;

          &:hover {
            background-image: url(@/assets/home/home-news-tree-hover.jpg);
            & > .home-news__block-box__item-grayscale {
              background: $grayscale-gradient;
            }
          }
        }

        &.--4 {
          height: 244px;
          background: $grey-gradient;
          background-size: cover;

          &:hover {
            background-image: url(@/assets/home/home-news-four-hover.jpg);
            & > .home-news__block-box__item-grayscale {
              background: $grayscale-gradient;

              & > .home-news__block-box__item-title {
                color: $white !important;
              }
            }
          }
        }

        &.--5 {
          height: 284px;
          background-image: url(@/assets/home/home-news-five.svg);
          background-size: cover;

          &:hover {
            background-image: url(@/assets/home/home-news-five-hover.jpg);
            & > .home-news__block-box__item-grayscale {
              background: $grayscale-gradient;

              & > .home-news__block-box__item-title {
                color: $white !important;
              }
            }
          }
        }

        &.--6 {
          height: 126px;
          background: $grey-gradient;
          background-size: cover;

          &:hover {
            background-image: url(@/assets/home/home-news-six-hover.jpg);
            & > .home-news__block-box__item-grayscale {
              background: $grayscale-gradient;

              & > .home-news__block-box__item-title {
                color: $white !important;
              }
            }
          }
        }

        &.--7 {
          height: 218px;
          background: $grey-gradient;
          background-size: cover;

          &:hover {
            background-image: url(@/assets/home/home-news-seven-hover.jpg);
            & > .home-news__block-box__item-grayscale {
              background: $grayscale-gradient;

              & > .home-news__block-box__item-title {
                color: $white !important;
              }
            }
          }
        }

        &.--8 {
          height: 194px;
          background-color: $red;
          background-size: cover;

          &:hover {
            background-image: url(@/assets/home/home-news-eight-hover.jpg);
            & > .home-news__block-box__item-grayscale {
              background: $grayscale-gradient;
            }
          }
        }
      }
    }
  }
}
</style>
