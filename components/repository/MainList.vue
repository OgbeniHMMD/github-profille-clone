<template>
  <main>
    <article v-for="i in 5" :key="i" class="repo-article">
      <div class=" ">
        <h3 class="title">
          <a href="/OgbeniHMMD/chat-app"> chat-app</a>
        </h3>

        <div></div>

        <div class="repo-subtitle">
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
                  fill="d1d5da"
                  d="M5 3.25a.75.75 0 11-1.5 0 .75.75 0 011.5 0zm0 2.122a2.25 2.25 0 10-1.5 0v.878A2.25 2.25 0 005.75 8.5h1.5v2.128a2.251 2.251 0 101.5 0V8.5h1.5a2.25 2.25 0 002.25-2.25v-.878a2.25 2.25 0 10-1.5 0v.878a.75.75 0 01-.75.75h-4.5A.75.75 0 015 6.25v-.878zm3.75 7.378a.75.75 0 11-1.5 0 .75.75 0 011.5 0zm3-8.75a.75.75 0 100-1.5.75.75 0 000 1.5z"
                ></path>
              </svg>
              2
            </a>
          </span>

          <span class="span">
            <svg
              class="octicon octicon-law mr-1"
              viewBox="0 0 16 16"
              version="1.1"
              width="16"
              height="16"
              aria-hidden="true"
            >
              <path
                fill="d1d5da"
                d="M8.75.75a.75.75 0 00-1.5 0V2h-.984c-.305 0-.604.08-.869.23l-1.288.737A.25.25 0 013.984 3H1.75a.75.75 0 000 1.5h.428L.066 9.192a.75.75 0 00.154.838l.53-.53-.53.53v.001l.002.002.002.002.006.006.016.015.045.04a3.514 3.514 0 00.686.45A4.492 4.492 0 003 11c.88 0 1.556-.22 2.023-.454a3.515 3.515 0 00.686-.45l.045-.04.016-.015.006-.006.002-.002.001-.002L5.25 9.5l.53.53a.75.75 0 00.154-.838L3.822 4.5h.162c.305 0 .604-.08.869-.23l1.289-.737a.25.25 0 01.124-.033h.984V13h-2.5a.75.75 0 000 1.5h6.5a.75.75 0 000-1.5h-2.5V3.5h.984a.25.25 0 01.124.033l1.29.736c.264.152.563.231.868.231h.162l-2.112 4.692a.75.75 0 00.154.838l.53-.53-.53.53v.001l.002.002.002.002.006.006.016.015.045.04a3.517 3.517 0 00.686.45A4.492 4.492 0 0013 11c.88 0 1.556-.22 2.023-.454a3.512 3.512 0 00.686-.45l.045-.04.01-.01.006-.005.006-.006.002-.002.001-.002-.529-.531.53.53a.75.75 0 00.154-.838L13.823 4.5h.427a.75.75 0 000-1.5h-2.234a.25.25 0 01-.124-.033l-1.29-.736A1.75 1.75 0 009.735 2H8.75V.75zM1.695 9.227c.285.135.718.273 1.305.273s1.02-.138 1.305-.273L3 6.327l-1.305 2.9zm10 0c.285.135.718.273 1.305.273s1.02-.138 1.305-.273L13 6.327l-1.305 2.9z"
              ></path></svg
            >MIT License
          </span>

          <span class="span">
            Updated
            <time datetime="2021-01-18T09:47:43Z" class="no-wrap"
              >Jan 18, 2021</time
            >
          </span>
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
  </main>
</template>

<style scoped>
.repo-article {
  border-top: 1px solid var(--border-color);
  padding: 1.5em 0;
  color: var(--grey);
}

.repo-subtitle span {
  padding-right: 1em;
}

.title {
  display: block;
  letter-spacing: 1px;
  padding-bottom: 1em;
}
</style>
