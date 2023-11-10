<template>
  <section class="home-news mt-6">
    <v-container>
      <div class="home-news__block d-flex flex-wrap justify-center">
        <div class="home-news__block-box --big mr-8">
          <div class="home-news__block-box__item --1">
            <div class="home-news__block-box__item-grayscale pa-5">
              <p class="home-news__block-box__item-title size-parag">
                Об университете
              </p>
            </div>
          </div>
          <div class="home-news__block-box__item --2 mt-8">
            <div class="home-news__block-box__item-grayscale pa-5">
              <p
                class="home-news__block-box__item-title color-white size-parag"
              >
                Образование
              </p>
            </div>
          </div>
        </div>
        <div class="home-news__block-box --min mr-8">
          <div class="home-news__block-box__item --3">
            <div class="home-news__block-box__item-grayscale pa-5">
              <p
                class="home-news__block-box__item-title color-white size-parag"
              >
                Наука и инновации
              </p>
            </div>
          </div>
          <div class="home-news__block-box__item --4 mt-8">
            <div class="home-news__block-box__item-grayscale pa-5">
              <p class="home-news__block-box__item-title size-parag">
                Приоритет 2030
              </p>
            </div>
          </div>
        </div>
        <div class="home-news__block-box --big mr-8">
          <div class="home-news__block-box__item --5">
            <div class="home-news__block-box__item-grayscale pa-5">
              <p class="home-news__block-box__item-title size-parag">
                Молодежная политика
              </p>
            </div>
          </div>
          <div class="home-news__block-box__item --6 mt-8">
            <div class="home-news__block-box__item-grayscale pa-5">
              <p class="home-news__block-box__item-title size-parag">
                Контакты
              </p>
            </div>
          </div>
        </div>
        <div class="home-news__block-box --min mr-8">
          <div class="home-news__block-box__item --7">
            <div class="home-news__block-box__item-grayscale pa-5">
              <p class="home-news__block-box__item-title size-parag">
                Брендбук
              </p>
            </div>
          </div>
          <div class="home-news__block-box__item --8 mt-8">
            <div class="home-news__block-box__item-grayscale pa-5">
              <p
                class="home-news__block-box__item-title color-white size-parag"
              >
                Приёмная комиссия
              </p>
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
        max-width: 336px;
        width: 100%;
      }

      &.--min {
        max-width: 192px;
        width: 100%;
      }

      &__item {
        border-radius: 20px;

        &-grayscale {
          width: 100%;
          height: 100%;
          border-radius: 20px;
        }

        &.--1 {
          height: 214px;
          background-image: url(../../../public/assets/home/home-news-first.svg);

          &:hover {
            background-image: url(../../../public/assets/home/home-news-first-hover.jpg);
            & > .home-news__block-box__item-grayscale {
              background: $grayscale-gradient;
            }
          }
        }

        &.--2 {
          height: 192px;
          background-color: $main-blue;
          background-image: url(../../../public/assets/home/home-news-two.svg);
          background-position: 105% 105%;

          &:hover {
            background-image: url(../../../public/assets/home/home-news-two-hover.jpg);
            & > .home-news__block-box__item-grayscale {
              background: $grayscale-gradient;
            }
          }
        }

        &.--3 {
          height: 164px;
          background: linear-gradient(180deg, $main-blue 0%, $main-blue 100%);

          &:hover {
            background-image: url(../../../public/assets/home/home-news-tree-hover.jpg);
            & > .home-news__block-box__item-grayscale {
              background: $grayscale-gradient;
            }
          }
        }

        &.--4 {
          height: 244px;
          background: $grey-gradient;

          &:hover {
            background-image: url(../../../public/assets/home/home-news-four-hover.jpg);
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
          background-image: url(../../../public/assets/home/home-news-five.svg);

          &:hover {
            background-image: url(../../../public/assets/home/home-news-five-hover.jpg);
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

          &:hover {
            background-image: url(../../../public/assets/home/home-news-six-hover.jpg);
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

          &:hover {
            background-image: url(../../../public/assets/home/home-news-seven-hover.jpg);
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

          &:hover {
            background-image: url(../../../public/assets/home/home-news-eight-hover.jpg);
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
