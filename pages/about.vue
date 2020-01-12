<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="About Me"
      subtitle="A few words about the author of this blog"
      image="https://picsum.photos/1800/1801"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h2>The nice things about blogs...</h2>
          <p>
            <strong>You can write anything you want, all is allowed.</strong>
          </p>
          <h3>A bit about me</h3>
          <p>
            I am a software developer and my experience has been on the
            <strong>reporting arena.</strong> I started very long time ago
            trying to implement reporting techniques to produce printed books
            like directories using data from external systems, importing data to
            Mac computers and make final art for printing.
          </p>
          <p>
            Since then I have developed hundreds of reporting systems, including
            visualization tools, ETL techniques, standard reports with drill
            down capabilities, an a lot of things I would like to share.
          </p>
          <p>
            Computer programming is now days the fusion of Technique and Art.
            This blog is not intended for newcomers as reporting is a serious
            business, but I wil try to keep it as simple as possible so you can
            get some ideas out of it.
          </p>

          <h3>Mentorship & teaching</h3>
          <p>
            I like to teach people how to program, and I do this in several
            ways. When it comes to formal courses I work with
            <strong>cusosgerenciales.com</strong>. You can find there basically
            my Office related courses. I have a free program for educators that
            we are promoting via the
            <strong>Venezuelan Natural Science Society.</strong> And I mentor
            individual students so that they can accomplish a long term career
            in this industry.
          </p>

          <h3>Development</h3>
          <p>
            Currently I lead the Development team at
            <strong>Maprotel,</strong> a callcenter consulting agency, and the
            core product that is
            <strong>Proser.</strong>
          </p>

          <h3>Tech Stack</h3>
          <p>
            Now days I focus on Javascript/Typescript ecosystem. This means I
            use things like Angular, React, Vue in the frontend and Node for
            backend including frameworks and libraries like Express, Koa,
            Loopback and many others.
          </p>
          <p>
            On the persistance layer I am devoted to MariaDB, a drop in
            replacement for MySQL, but also like NoSQL databases like Mongo,
            Arango and CouchDB.
          </p>
          <p>
            We are pointing to serverless architectures the JamStack and some
            other cool technologies for future projects.
          </p>
        </div>
      </template>

      <template v-slot:sidebar>
        <h3 class="subtitle is-4">Latest Posts</h3>
        <posts-grid :per-row="1" :number="2" />
      </template>
    </main-section>
  </div>
</template>
<script>
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  }
}
</script>

<style scoped>
h3 {
  font-size: 1.8rem;
}
p {
  font-size: 1.5rem;
}
</style>
