<script setup>

import Partner from "@/components/Home/Partner.vue";
import {ref} from "vue";

const email = ref('')
const submit = () => {
  email.value = ''
  alert('success');
}
// https://glassnode.com/
</script>

<template>
  <main>
    <div class="header shadow  flex items-center">
      <div class="content flex items-center justify-between flex-1">
        <h1 class="text-xl font-bold">Norton Fund</h1>
        <div class="right text-lg text-blue-500">
          <a href="https://norton.im/download/android">App下载</a>
        </div>
      </div>
    </div>

    <div class="section">
      <div class="content">

        <div class="view">

          <div class="left xl:w-1/2">
            <div class="title1 text-4xl font-semibold py-8 mt-8 leading-tight">
              Stay ahead of the trend in digital assets
            </div>
            <div class="title2 leading-7">
              Norton empowers traders and investors to anticipate the core trends and inflection points moving digital assets. We specialise in providing sophisticated blockchain
              and market data, offering unique insights into capital flows, asset fundamentals, and market sentiment in Bitcoin and Ethereum.
            </div>
          </div>
          <div class="right">
            <img src="@/assets/images/canvas.png" alt="">
          </div>
        </div>

        <div class="flex justify-center text-3xl font-serif mt-20">
          As seen on
        </div>
        <Partner></Partner>

        <div class="view view2 xl:items-center">

          <div class="left xl:w-1/2 xl:flex-shrink-0 xl:p-6">
            <div class="title1 text-2xl font-semibold  py-8 mt-8 leading-tight">
              Capitalize on premier on-chain and financial market data
            </div>
            <div class="title2 leading-7">
              Empower your decision-making with thousands of metrics and indicators for Bitcoin, Ethereum, DeFi, stablecoins, top cryptocurrencies, and derivatives markets.
            </div>
            <div class="flex flex-col icons">
              <div class="item flex">
                <img class="" src="@/assets/images/icons/chart-line-smooth-icon.8cc62ea0.svg" alt="">
                <div>Unrivalled on-chain metric depth and data science methodology</div>
              </div>
              <div class="item flex">
                <img src="@/assets/images/icons/data-format-icon.577b6c5e.svg" alt="">
                <div>Precise wallet tracking via proprietary clustering algorithms</div>
              </div>
              <div class="item flex">
                <img src="@/assets/images/icons/data-exchange-icon.7304cd7f.svg" alt="">
                <div>Comprehensive exchange data coverage</div>
              </div>
              <div class="item flex">
                <img src="@/assets/images/icons/realtime-data-icon.f32bf755.svg" alt="">
                <div>High performance API and intuitive charting suite</div>
              </div>
            </div>
          </div>
          <div class="right xl:p-6 xl:w-1/2">
            <img src="@/assets/images/chains.webp" alt="">
          </div>
        </div>

        <div class="view view2 xl:items-center">
          <div class="left xl:p-6 xl:w-1/2">
            <img src="@/assets/images/graphs-en.webp" alt="">
          </div>
          <div class="right xl:w-1/2 xl:flex-shrink-0 xl:p-6">
            <div class="title1 text-2xl font-semibold  py-8 mt-8 leading-tight">
              Cut through the noise and discover unique market insights
            </div>
            <div class="title2 leading-7">
              Gain the knowledge and confidence to make data-driven decisions with our tailor-made tools and expert market analysis.
            </div>
            <div class="flex flex-col icons">
              <div class="item flex">
                <img class="" src="@/assets/images/icons/dashboard-icon.2b376f1d.svg" alt="">
                <div>Curated dashboards for instant market evaluation</div>
              </div>
              <div class="item flex">
                <img src="@/assets/images/icons/article-icon.ae74fec0.svg" alt="">
                <div>Cutting-edge research and market updates</div>
              </div>
              <div class="item flex">
                <img src="@/assets/images/icons/chart-icon.2a605b4d.svg" alt="">
                <div>High-signal charts and custom indicators</div>
              </div>
            </div>
          </div>
        </div>

      </div>
    </div>

    <div class="section bg-[#f7f8fa]">
      <div class="card">
        <div class="title">Get access to Norton</div>
        <div class="sub-title mt-4">Take the next step and discover the power of blockchain intelligence.</div>
      </div>
    </div>

    <footer class="footer">
      <div class="content">
        <div class="subscribe">
          <div class="text-2xl font-semibold mb-2 text-white">Subscribe to our newsletter</div>
          <div class="my-2">Receive weekly expert market analysis, best-in-class research on Bitcoin, Ethereum, DeFi, & more.</div>
          <div class="input flex my-2">
            <input type="text" class="input" placeholder="Enter your email" v-model="email">
            <button type="button" class="btn" @click="submit">submit</button>
          </div>
        </div>
        <div class="subscribe" style="margin-top: 20px">
          <div class="text-2xl font-semibold mb-2 text-white">Contact Us</div>
          <div class="my-2 text-white">Ask questions and request support</div>
          <div class="my-2 text-blue-500">
            <a href="mailto:norton@nt-fund.com">norton@nt-fund.com</a>
          </div>
        </div>
        <hr class="text-[#eee] mt-10">
        <div class="copyright mt-10 text-white pb-10">
          <div>
            © 2024 THIRTIES ROOM. COMPANY LIMITED, all rights reserved
          </div>
        </div>
      </div>
    </footer>
  </main>
</template>

<style lang="less">
.header {
  background: white;
  height: 71px;
  width: 100%;
}

.section {
  .content {
    .view {
      display: flex;
      flex-direction: column;
    }
  }

  .card {
    padding: 40px;

    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
  }
}

.title {
  font-size: 32px;
  font-weight: 600;
}

.sub-title {
  color: rgb(90, 90, 90);
}

.header, .section {
  .content {
    //margin: .75rem auto;
    padding: .75rem;
  }
}

.view2 {
  .title2 {
    color: rgb(90, 90, 90);
  }

  .icons {
    color: rgb(90, 90, 90);
  }

  .item {
    //line-height: 200%;
    margin: 10px 0;

    img {
      margin-right: 10px;


      width: 20px;
      height: 20px;
    }
  }
}

.footer {
  background: #000;
  padding: .75rem;

  .input {
    display: flex;
    align-items: center;

    .input {
      width: 326px;
      height: 40px;
      padding-left: 10px;

      background: transparent;

      border: 1px solid rgb(128, 128, 128);

      border-bottom-left-radius: 4px;
      border-top-left-radius: 4px;
    }

    .btn {
      display: inline-block;
      background-color: white;
      border: 1px solid #bfbfbf;
      cursor: pointer;
      font-size: .875rem;
      line-height: 1.3;
      text-align: center;
      transition: all .2s cubic-bezier(.645, .045, .355, 1);
      border-radius: 0 .125rem .125rem 0;
      padding: .6rem 1rem;
      color: #333;
    }
  }
}

@media (min-width: 1280px) {
  .header {
    height: 97px;
  }

  .header, .section {
    .content {
      max-width: 1280px;
      margin: 0 auto;
      padding: 0;

      .view {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
      }
    }
  }

  .section {
    background: linear-gradient(#edeff2, rgba(237, 239, 242, 0));
  }

  .footer {
    padding: 100px 40px;

    .content {
      max-width: 1280px;
      margin: 0 auto;
      padding: 0;

      color: rgb(222, 223, 225);

      .subscribe {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;


      }
    }
  }

}
</style>
