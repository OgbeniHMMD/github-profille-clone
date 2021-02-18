<template>
  <aside>
    <section v-if="userData">
      <div>
        <div style="z-index: 4; margin-top: -1.5em">
          <img
            style="height: auto; border-radius: 50%"
            alt="Avatar"
            width="260"
            height="260"
            class="avatar avatar-user width-full border bg-white"
            :src="userData.avatar_url"
          />
        </div>

        <h1 class="vcard-names">
          <div class="vcard-fullname overflow-hidden" itemprop="name">
            {{ userData.name }}
          </div>
          <div class="link-gray">
            {{ userData.login }}
          </div>
        </h1>
      </div>

      <div>
        <div>
          <div>
            <a class="link-gray" href="/#!/followers">
              <svg
                class="octicon octicon-people text-gray-light"
                height="16"
                viewBox="0 0 16 16"
                version="1.1"
                width="16"
                aria-hidden="true"
              >
                <path
                  fill="grey"
                  fill-rule="evenodd"
                  d="M5.5 3.5a2 2 0 100 4 2 2 0 000-4zM2 5.5a3.5 3.5 0 115.898 2.549 5.507 5.507 0 013.034 4.084.75.75 0 11-1.482.235 4.001 4.001 0 00-7.9 0 .75.75 0 01-1.482-.236A5.507 5.507 0 013.102 8.05 3.49 3.49 0 012 5.5zM11 4a.75.75 0 100 1.5 1.5 1.5 0 01.666 2.844.75.75 0 00-.416.672v.352a.75.75 0 00.574.73c1.2.289 2.162 1.2 2.522 2.372a.75.75 0 101.434-.44 5.01 5.01 0 00-2.56-3.012A3 3 0 0011 4z"
                ></path>
              </svg>
              <strong class="text-gray-dark"> {{ userData.followers }}</strong>
              followers
            </a>
            &middot;
            <a class="link-gray" href="/#!/following">
              <strong class="text-gray-dark"> {{ userData.following }}</strong>
              following
            </a>
            &middot;
            <a class="link-gray" href="/#!/stars">
              <svg
                class="octicon octicon-star text-gray-light"
                height="16"
                viewBox="0 0 16 16"
                version="1.1"
                width="16"
                aria-hidden="true"
              >
                <path
                  fill-rule="evenodd"
                  d="M8 .25a.75.75 0 01.673.418l1.882 3.815 4.21.612a.75.75 0 01.416 1.279l-3.046 2.97.719 4.192a.75.75 0 01-1.088.791L8 12.347l-3.766 1.98a.75.75 0 01-1.088-.79l.72-4.194L.818 6.374a.75.75 0 01.416-1.28l4.21-.611L7.327.668A.75.75 0 018 .25zm0 2.445L6.615 5.5a.75.75 0 01-.564.41l-3.097.45 2.24 2.184a.75.75 0 01.216.664l-.528 3.084 2.769-1.456a.75.75 0 01.698 0l2.77 1.456-.53-3.084a.75.75 0 01.216-.664l2.24-2.183-3.096-.45a.75.75 0 01-.564-.41L8 2.694v.001z"
                ></path>
              </svg>
              <strong class="text-gray-dark">50</strong>
            </a>
          </div>
        </div>

        <div class="vcard-details">
          <div class="vcard-detail" itemprop="homeLocation" show_title="false">
            <svg
              viewBox="0 0 16 16"
              version="1.1"
              width="16"
              height="16"
              aria-hidden="true"
            >
              <path
                fill="grey"
                fill-rule="evenodd"
                d="M11.536 3.464a5 5 0 010 7.072L8 14.07l-3.536-3.535a5 5 0 117.072-7.072v.001zm1.06 8.132a6.5 6.5 0 10-9.192 0l3.535 3.536a1.5 1.5 0 002.122 0l3.535-3.536zM8 9a2 2 0 100-4 2 2 0 000 4z"
              ></path>
            </svg>
            <span class="p-label">{{ userData.location }}</span>
          </div>
          <div
            v-if="userData.email"
            itemprop="email"
            aria-label="Email: "
            class="vcard-detail pt-1 css-truncate css-truncate-target"
          >
            <svg
              class="octicon octicon-mail"
              viewBox="0 0 16 16"
              version="1.1"
              width="16"
              height="16"
              aria-hidden="true"
            >
              <path
                fill="grey"
                fill-rule="evenodd"
                d="M1.75 2A1.75 1.75 0 000 3.75v.736a.75.75 0 000 .027v7.737C0 13.216.784 14 1.75 14h12.5A1.75 1.75 0 0016 12.25v-8.5A1.75 1.75 0 0014.25 2H1.75zM14.5 4.07v-.32a.25.25 0 00-.25-.25H1.75a.25.25 0 00-.25.25v.32L8 7.88l6.5-3.81zm-13 1.74v6.441c0 .138.112.25.25.25h12.5a.25.25 0 00.25-.25V5.809L8.38 9.397a.75.75 0 01-.76 0L1.5 5.809z"
              ></path>
            </svg>
            <a rel="nofollow" class="link-gray-dark">{{ userData.email }}</a>
          </div>
          <div
            v-if="userData.blog"
            itemprop="url"
            data-test-selector="profile-website-url"
            class="vcard-detail pt-1 css-truncate css-truncate-target"
          >
            <svg
              class="octicon octicon-link"
              viewBox="0 0 16 16"
              version="1.1"
              width="16"
              height="16"
              aria-hidden="true"
            >
              <path
                fill="grey"
                fill-rule="evenodd"
                d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"
              ></path>
            </svg>
            <a
              rel="nofollow me"
              class="link-gray-dark"
              href="http://www.hmmd.xyz"
              >{{ userData.blog }}</a
            >
          </div>
          <div
            v-if="userData.twitter_username"
            class="vcard-detail"
            itemprop="twitter"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 273.5 222.3"
              class="octicon"
              width="16"
              height="16"
            >
              <path
                fill="grey"
                fill-rule="evenodd"
                d="M273.5 26.3a109.77 109.77 0 0 1-32.2 8.8 56.07 56.07 0 0 0 24.7-31 113.39 113.39 0 0 1-35.7 13.6 56.1 56.1 0 0 0-97 38.4 54 54 0 0 0 1.5 12.8A159.68 159.68 0 0 1 19.1 10.3a56.12 56.12 0 0 0 17.4 74.9 56.06 56.06 0 0 1-25.4-7v.7a56.11 56.11 0 0 0 45 55 55.65 55.65 0 0 1-14.8 2 62.39 62.39 0 0 1-10.6-1 56.24 56.24 0 0 0 52.4 39 112.87 112.87 0 0 1-69.7 24 119 119 0 0 1-13.4-.8 158.83 158.83 0 0 0 86 25.2c103.2 0 159.6-85.5 159.6-159.6 0-2.4-.1-4.9-.2-7.3a114.25 114.25 0 0 0 28.1-29.1"
              ></path>
            </svg>

            <a
              rel="nofollow me"
              class="link-gray-dark"
              :href="'https://twitter.com/' + userData.twitter_username"
              >@ {{ userData.twitter_username }}
            </a>
          </div>
        </div>
      </div>
    </section>
  </aside>
</template>

<script>
export default {
  data() {
    return {
      USERNAME: 'OgbeniHMMD',
      userData: null,
    }
  },

  created() {
    this.fetchUserInfo()
  },

  methods: {
    async fetchUserInfo() {
      const URI = `/users/${this.USERNAME}`
      await this.$axios
        .$get(URI)
        .then((response) => {
          console.log(response)
          this.userData = response
        })
        .catch((error) => {
          console.log(error)
        })
    },
  },
}
</script>

<style scoped>
.link-gray {
  color: var(--grey);
}
.link-gray-dark {
  color: var(--black);
}

.vcard-detail {
  padding-top: 0.5em;
}
.vcard-names {
  padding: 1em 0;
}
</style>
