<template>
  <main>
    <partials-app-bar />

    <article v-for="i in 5" :key="i" class="repo-article">
      <div class=" ">
        <h3 class="title">
          <a href="/OgbeniHMMD/chat-app"> chat-app</a>
        </h3>

        <div></div>

        <div>
          <span class="span">Vue</span>

          <span class="span">
            <a class=" " href="/OgbeniHMMD/chat-app/network/members">
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
          </span>

          <soan class="span">
            Updated
            <time datetime="2021-01-18T09:47:43Z" class="no-wrap"
              >Jan 18, 2021</time
            >
          </soan>
        </div>
      </div>

      <div class="col-2 col-lg-3 d-flex flex-column flex-justify-around">
        <!-- <div class="text-right hide-lg hide-md hide-sm hide-xs mt-2">
          <poll-include-fragment
            src="/OgbeniHMMD/chat-app/graphs/participation?w=155&amp;h=28&amp;type=sparkline)"
          >
          </poll-include-fragment>
        </div> -->
      </div>
    </article>

    <partials-footer />
  </main>
</template>

<style>
.repo-article {
  border-top: 1px solid var(--border-color);
  padding: 2em 0;
  margin: 1em 0;
  color: var(--grey);
}

,
.span {
  padding: 0 1.5em !important;
}

,
.containerx {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  display: block;
  letter-spacing: 1px;
  padding-bottom: 1em;
}
</style>
