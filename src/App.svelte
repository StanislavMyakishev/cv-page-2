<script lang="ts">
  import LinksTable from "./LinksTable.svelte";
  type PrefixType = "eng" | "ru";
  const getFileLink = (prefix: PrefixType) => `https://github.com/stanislavmyakishev/cv-page-2/raw/main/${prefix}_cv_myakishev.pdf`;
  const fileName = 'myakishev_stanislav_cv.pdf';
</script>

<style lang="scss">
  main {
    max-width: 800px;
    margin: 0 auto;
  }

  .content {
    margin: 130px 0 80px 0;
    text-align: center;
  }

  span, q {
    font-size: 22px;
    margin-bottom: 10px;
    line-height: 40px;
  }

  a {
    text-decoration: none;
    color: #000;
    font-weight: bold;
    transition: 0.3s;
  }

  .highlighted {
    background-color: #1A6DBB;
    color: #fff;
  }

  .highlight-link {
    background-color: #ff026fb3;
    color: #fff;
    transition: 0.3s;

    &:hover {
      color: #fff;
      transition: 0.3s;
    }
  }
</style>

<main>
  <div class="content">
    <span>Hi!</span>
    <br />
    <span>
      My name is&nbsp;
      <span class="highlighted">Stanislav Myakishev</span>
      &nbsp;and I'm a&nbsp;
      <span class="highlighted">front end developer</span>.
    </span>
    <br />
    <q>Brevity is the sister of talent</q>
      <figure>
        <figcaption>
          &mdash; Anton Chekhov
        </figcaption>
      </figure>
    <br />
    <span>
      So instead of many words here you can find my CV
      <br />
      in&nbsp;
      <a
        href={getFileLink('eng')}
        download={fileName}>
        <span class="highlight-link">english</span>
      </a>
      &nbsp;or in&nbsp;
      <a
        href={getFileLink('ru')}
        download={fileName}>
        <span class="highlight-link">russian</span>
      </a>
      .
    </span>
    <LinksTable />
  </div>
</main>
