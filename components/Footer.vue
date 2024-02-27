<template>
  <div class="footer">
    <div class="content">
      <div class="content1">
        <div class="img">
          <div class="contain">
            <img src="/assets/images/Logo.png" alt="website logo" class="" />
          </div>
          <span>Savings, Payments, Loans</span>
        </div>
        <div class="menu">
          <h2 class="menuh1">Quick</h2>
          <ul class="ul">
            <li>
              <NuxtLink to="">Our Story</NuxtLink>
            </li>
            <li>
              <NuxtLink to="">FAQs</NuxtLink>
            </li>
            <li>
              <NuxtLink to="">Media</NuxtLink>
            </li>
          </ul>
        </div>
        <div class="menu">
          <h2 class="menuh1">Legals</h2>
          <ul class="ul">
            <li>
              <NuxtLink to="">Terms & Conditions</NuxtLink>
            </li>
            <li>
              <NuxtLink to="">Privacy Policy</NuxtLink>
            </li>
          </ul>
        </div>
        <div class="menu">
          <h2 class="menuh1">Contact Us</h2>
          <div class="ul">
            <div class="contacts">
              <span class="">
                <img src="/assets/images/Vector2.png" alt="" />
              </span>
              <span class="break-all">
                UAC Building, 1-5 Odunlami St, Lagos Island, Lagos
              </span>
            </div>
            <div class="contacts">
              <span class="">
                <img src="/assets/images/Vector.png" alt="" />
              </span>
              <span>+234 812 345 6789</span>
            </div>
            <div class="contacts">
              <span class="">
                <img src="/assets/images/mail 1.png" alt="" />
              </span>
              <span>hello@vale.ng</span>
            </div>
            <div class="socials">
              <span class="">
                <img src="/assets/images/Vector3.png" alt="" />
              </span>
              <span class="">
                <img src="/assets/images/Vector4.png" alt="" />
              </span>
              <span class="">
                <img src="/assets/images/bxl-twitter.svg.png" alt="" />
              </span>
              <!-- <span class="">
                <img src="/assets/images/bxl-whatsapp-square.svg.png" alt="" />
              </span> -->
            </div>
          </div>
        </div>
        <div class="menu">
          <h2 class="menuh1">Contact Us</h2>
          <div class="ul">
            <div class="contacts">
              <span class="">
                <img src="/assets/images/Vector2.png" alt="" />
              </span>
              <span class="break-all">
                UAC Building, 1-5 Odunlami St, Lagos Island, Lagos
              </span>
            </div>
            <div class="contacts">
              <span class="">
                <img src="/assets/images/Vector.png" alt="" />
              </span>
              <span>+234 812 345 6789</span>
            </div>
            <div class="contacts">
              <span class="">
                <img src="/assets/images/mail 1.png" alt="" />
              </span>
              <span>hello@vale.ng</span>
            </div>
            <div class="socials">
              <span class="">
                <img src="/assets/images/Vector3.png" alt="" />
              </span>
              <span class="">
                <img src="/assets/images/Vector4.png" alt="" />
              </span>
              <span class="">
                <img src="/assets/images/bxl-twitter.svg.png" alt="" />
              </span>
              <!-- <span class="">
                <img src="/assets/images/bxl-whatsapp-square.svg.png" alt="" />
              </span> -->
            </div>
          </div>
        </div>
      </div>
      <div
        class="hidden md:block border-top border-white w-full border-[1px]"
      ></div>
      <p class="hidden md:block">
        Vale is a Mobile Bank provider, regulated by the Central Bank of
        Nigeria(CBN). Dollar investments are offered under a reseller
        partnership with Anchoria Asset Management Limited – a SEC-licensed
        asset management company. Deposit accounts are issued and managed by
        CBN-licensed deposit money banks
      </p>
      <span class="text-center md:text-left">
        2019 © All rights reserved by Vale Finance
      </span>
    </div>
  </div>
</template>

<script setup>
</script>

<style lang="scss" scoped>
.footer {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: #0267fd;
  padding-top: 2.25rem; /* 9/4 = 2.25rem */
  padding-bottom: 2.25rem;
  margin-top: 2.25rem;
  .content {
    width: 85%;
    color: white;
    display: flex;
    justify-content: center;
    flex-direction: column;
    row-gap: 3rem;

    .content1 {
      display: grid;
      grid-template-columns: repeat(5, minmax(0, 1fr));
      row-gap: 2.5rem;

      .menu {
        display: flex;
        flex-direction: column;
        row-gap: 1.5rem;
        .menuh1 {
          font-weight: 700;
        }
        .ul {
          display: flex;
          flex-direction: column;
          row-gap: 0.75rem;
        }
        .contacts {
          display: flex;
          align-items: center;
          width: 100%;
          gap: 1rem;
          font-size: 1.125rem /* 18px */;
          line-height: 1.75rem /* 28px */;
        }
        .socials {
          display: flex;
          align-items: center;
          width: 100%;
          gap: 0.5rem;
        }
      }
    }
    @media (max-width: 767px) {
      .content1 {
        display: grid;
        grid-template-columns: repeat(1, minmax(0, 1fr));
        row-gap: 2.5rem;
      }
    }
    @media (min-width: 768px) and (max-width: 992px) {
      .content1 {
        display: grid;
        grid-template-columns: repeat(2, minmax(0, 1fr));
      }
      .menu {
        display: flex;
        flex-direction: column;
        row-gap: 0.75rem;
      }
    }
    @media (min-width: 993px) {
      .content1 {
        display: grid;
        grid-template-columns: repeat(5, minmax(0, 1fr));
        row-gap: 2.5rem;
      }
    }
    .img {
      width: 100%;
      .contain {
        width: 50%;
        img {
          object-fit: contain;
          width: 50%;
        }
      }
    }
  }
}
</style>