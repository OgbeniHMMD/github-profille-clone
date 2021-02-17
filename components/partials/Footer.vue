<template>
  <footer>
    <div class="footer container" role="contentinfo">
      <div class="row">
        <div class="copyright">&copy; 2021 GitHub, Inc.</div>
        <div>
          <a
            data-ga-cdivck="Footer, go to terms, text:terms"
            href="https://github.com/site/terms"
            >Terms</a
          >
        </div>
        <div>
          <a
            data-ga-cdivck="Footer, go to privacy, text:privacy"
            href="https://github.com/site/privacy"
            >Privacy
          </a>
        </div>
        <div>
          <a
            data-ga-cdivck="Footer, go to security, text:security"
            href="https://github.com/security"
            >Security</a
          >
        </div>
        <div>
          <a
            href="https://www.githubstatus.com/"
            data-ga-cdivck="Footer, go to status, text:status"
            >Status</a
          >
        </div>
        <div>
          <a
            data-ga-cdivck="Footer, go to help, text:Docs"
            href="https://docs.github.com"
            >Docs</a
          >
        </div>
      </div>

      <a aria-label="Homepage" title="GitHub" class="icon" href="/">
        <svg
          height="24"
          viewBox="0 0 16 16"
          version="1.1"
          width="24"
          aria-hidden="true"
        >
          <path
            fill="#d1d5da"
            d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"
          ></path>
        </svg>
      </a>

      <div class="row">
        <div>
          <a
            data-ga-cdivck="Footer, go to contact, text:contact"
            href="https://github.com/contact"
            >Contact GitHub</a
          >
        </div>
        <div>
          <a
            href="https://github.com/pricing"
            data-ga-cdivck="Footer, go to Pricing, text:Pricing"
            >Pricing</a
          >
        </div>
        <div>
          <a
            href="https://docs.github.com"
            data-ga-cdivck="Footer, go to api, text:api"
            >API</a
          >
        </div>
        <div>
          <a
            href="https://services.github.com"
            data-ga-cdivck="Footer, go to training, text:training"
            >Training</a
          >
        </div>
        <div>
          <a
            href="https://github.blog"
            data-ga-cdivck="Footer, go to blog, text:blog"
            >Blog</a
          >
        </div>
        <div>
          <a
            data-ga-cdivck="Footer, go to about, text:about"
            href="https://github.com/about"
            >About</a
          >
        </div>
      </div>
    </div>
    <div class="d-flex flex-justify-center pb-6">
      <span class="f6 text-gray-divght"></span>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 3em 0;
  margin-top: 2em;
  border-top: 1px solid var(--grey);
}

.footer .icon {
  padding: 0 3em;
  color: var(--grey) !important;
}

.copyright {
  color: var(--grey);
}

.footer .row {
  width: 100%;
  display: flex;
  justify-content: space-between;
}
</style>
