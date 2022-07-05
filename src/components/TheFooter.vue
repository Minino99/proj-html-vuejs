<template>
  <div>
    <div class="container-fluid">
      <div class="container h-100">
        <div class="row h-100 align-items-center g-1">
          <div class="col">
            <div class="pb-4">
              <img
                src="images/logo.png"
                class="w-50"
                alt="NEXGEN logo"
                srcset=""
              />
            </div>
            <div class="text-white pb-4">
              A functional HTML Template for Corporate & business
            </div>
            <div class="pb-4">
              <div
                v-for="info in infos"
                :key="`footer-info-${info.name}`"
                class="text-white"
              >
                <i class="text-white pe-3 pb-2" :class="info.icon"></i>
                {{ info.name }}
              </div>
            </div>
            <div>
              <button class="btn btn-outline-primary btn-block text-white">
                GET IN TOUCH
              </button>
            </div>
          </div>

          <div
            class="col pe-4"
            v-for="element in footerElements"
            :key="element.title"
          >
            <div class="footerlinks p-5">
                <h4 class="pb-4 text-white">{{ element.title }}</h4>
                <div
                  v-for="link in element.links"
                  :key="link"
                  class="text-white pb-2"
                >
                  <i class="fa-solid fa-chevron-right text-white fs-5 pe-2"></i>
                  {{ link }}
                </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="container-fluid-endpage">
      <div
        class="container d-flex justify-content-between align-items-center h-100"
      >
        <div class="text-white">
          Enjoy the low price. We are tracking any intention of piracy
        </div>
        <div class="text-white">
          © 2020 NEXGEN is Proudly Powered by
          <span class="text-primary">Codings</span>.
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { state } from "@/store";

export default {
  name: "TheFooter",
  components: {},
  data: function () {
    return {
      infos: state.infos,
      footerElements: [
        {
          title: "About",
          links: [
            "The Company",
            "Institutional",
            "Social & Events",
            "Innovation",
            "Environment",
            "Technology",
          ],
        },
        {
          title: "Services",
          links: [
            "Audit & Assurance",
            "Financial Advisory",
            "Analytics M&A",
            "Middle Marketing",
            "Legal Consulting",
            "Regulatory Risk",
          ],
        },
        {
          title: "Support",
          links: [
            "Responsibility",
            "Terms of Use",
            "About Cookies",
            "Privacy Policy",
            "Accessibility",
            "Information",
          ],
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/variables.scss";

.footerlinks {
  background-color: #19191f;
  border-radius: 20px;
}
.container-fluid {
  background-color: #111117;
  height: 600px;
}

.container-fluid-endpage {
  background-color: #0d0d11;
  height: 90px;
}
</style>
