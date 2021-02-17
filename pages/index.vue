<template>
  <main>
    <partials-app-bar />

    <article
      v-for="i in 5"
      :key="i"
      class="col-12 d-flex width-full py-4 border-bottom color-border-secondary public source"
      itemprop="owns"
      itemscope
      itemtype="http://schema.org/Code"
    >
      <div class="col-10 col-lg-9 d-inline-block">
        <div class="d-inline-block mb-1">
          <h3 class="wb-break-all">
            <a href="/OgbeniHMMD/chat-app" itemprop="name codeRepository">
              chat-app</a
            >
          </h3>
        </div>

        <div></div>

        <div class="f6 text-gray mt-2">
          <span class="ml-0 mr-3">
            <span
              class="repo-language-color"
              style="background-color: #2c3e50"
            ></span>
            <span itemprop="programmingLanguage">Vue</span>
          </span>

          <a
            class="muted-link mr-3"
            href="/OgbeniHMMD/chat-app/network/members"
          >
            <svg
              aria-label="fork"
              class="octicon octicon-repo-forked"
              viewBox="0 0 16 16"
              version="1.1"
              width="16"
              height="16"
              role="img"
            >
              <path
                fill-rule="evenodd"
                d="M5 3.25a.75.75 0 11-1.5 0 .75.75 0 011.5 0zm0 2.122a2.25 2.25 0 10-1.5 0v.878A2.25 2.25 0 005.75 8.5h1.5v2.128a2.251 2.251 0 101.5 0V8.5h1.5a2.25 2.25 0 002.25-2.25v-.878a2.25 2.25 0 10-1.5 0v.878a.75.75 0 01-.75.75h-4.5A.75.75 0 015 6.25v-.878zm3.75 7.378a.75.75 0 11-1.5 0 .75.75 0 011.5 0zm3-8.75a.75.75 0 100-1.5.75.75 0 000 1.5z"
              ></path>
            </svg>
            2
          </a>

          Updated
          <relative-time datetime="2021-01-18T09:47:43Z" class="no-wrap"
            >Jan 18, 2021</relative-time
          >
        </div>
      </div>

      <div class="col-2 col-lg-3 d-flex flex-column flex-justify-around">
        <div class="text-right hide-lg hide-md hide-sm hide-xs mt-2">
          <poll-include-fragment
            src="/OgbeniHMMD/chat-app/graphs/participation?w=155&amp;h=28&amp;type=sparkline)"
          >
          </poll-include-fragment>
        </div>
      </div>
    </article>

    <partials-footer />
  </main>
</template>

<style>
.containerx {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
