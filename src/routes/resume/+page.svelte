<script>
  import HSep from "$lib/components/HSep.svelte";
  let title = "Keziah Hobbs";
  let subtitle = "Voice Actor";
</script>

<main>
  <header>
    <a href="/"><img src="/images/kat.jpg" alt="kat" /></a>
    <div class="right-matter">
      <section>
        <h1>Executive Summary</h1>
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Exercitationem
        animi nihil facilis?
      </section>
      <section>
        <h1>Contact</h1>
        Email:<a class="mail" href="mailto:k@keziah.ca">k@keziah.ca</a>
      </section>
    </div>
    <aside>
      <p>
        <a class="title" href="/">
          <h1>{title}</h1>
        </a>
      </p>
      <p>{subtitle}</p>
    </aside>
  </header>
  <HSep />
  <article>
    <div class="colored-box">
      <!-- <h1>Specializations</h1>
			<ul>
				<li>Lorem ipsum dolor sit</li>
				<li>amet consectetur adipisicing elit.</li>
				<li>Totam quam minus cum itaque magni</li>
				<li>eveniet corporis sequi?</li>
			</ul>
			<h1>Education</h1>
			<h2>Some school</h2>
			<ul>
				<li>Lorem ipsum dolor sit</li>
				<li>amet consectetur adipisicing elit.</li>
			</ul>
			<h2>A different school</h2>
			<ul>
				<li>Lorem ipsum dolor sit</li>
				<li>amet consectetur adipisicing elit.</li>
				<li>Totam quam minus cum itaque magni</li>
				<li>eveniet corporis sequi?</li>
			</ul> -->
      <p>
        Keziah Hobbs is a young Calgary-based voice actress specializing in
        character work and voice over.
      </p>

      <p>
        She is available for local studio work or can work remotely for national
        or international spots.
      </p>

      <p>
        If you need an exciting, fun, and nimble voice actor, Keziah is the
        perfect choice for your show or advertising spot.
      </p>

      <p>She’s also able to work as an extra.</p>
    </div>
    <div class="box">
      <h1>Career</h1>
      <ul>
        <li>Creepy voice: <i>Aria, SAIT Productions</i></li>
        <li>Klor: Rabbit Ears, <i>SC Entertainment</i></li>
        <li>
          Deeply Unimpressed Tavern Server: <i
            >+2 Rodcast, Tony Binns Producer</i
          >
        </li>
        <li>
          Narrator: <i>
            Narrator: Instructional Video, Southern Alberta Institute of
            Technology Narrator:
          </i>
        </li>
      </ul>
      <h1>Special Skills</h1>
      <ul>
        <li>Swimming</li>
        <li>Singing</li>
      </ul>
    </div>
  </article>
</main>

<style lang="scss">
  main {
    width: 42.5em;
    box-shadow: 0 0 5px 3px var(--secondary-light);
    border-radius: 5px 2em 5px 5px;
    margin: 1em auto;

    header {
      height: 15em;
      background-color: var(--primary);
      border-radius: 5px 2em 0 0;
      display: flex;
      position: relative;

      aside {
        position: absolute;
        top: 6em;
        left: 0;
        writing-mode: vertical-rl;
        color: var(--secondary-light);
        transform: rotate(180deg);
        font-variant: small-caps;

        p {
          /* font-size: 150%; */
          padding: 0;
          margin: 0;

          a {
            &:link,
            &:visited,
            &:active {
              color: var(--secondary);
              font-weight: bold;
              text-decoration: none;
            }
            &:hover {
              color: white;
            }
          }

          & + p {
            font-size: 120%;
            margin-right: -1em;
            color: var(--secondary);
          }
        }
      }

      img {
        margin-left: 5em;
        height: 100%;
      }

      .right-matter {
        padding: 1em;
        margin: 0 2em;
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        color: var(--secondary-light);

        h1 {
          margin: 0;
          padding: 0;
          font-variant: small-caps;
        }

        a.mail {
          color: var(--secondary-light);
          font-family: "Courier New", Courier, monospace;
          text-decoration: none;
        }
      }
    }

    article {
      display: flex;
      padding: 0;
      margin: 0;
    }

    .colored-box,
    .box {
      width: 45%;
      margin: 1em;
      padding: 1em;
      background-color: var(--secondary-light);

      h1 {
        color: var(--primary);
        font-variant: small-caps;
        font-size: 1.5rem;
        margin: 0;
        margin-bottom: 0.25em;
        padding: 0;

        & ~ h1 {
          margin-top: 1em;
        }

        // & ~ h2 {
        //   font-style: italic;
        //   color: var(--primary);
        //   font-size: 1.125rem;
        //   margin: 0.5em 0;
        // }
      }
    }

    .box {
      background-color: inherit;
    }

    ul {
      padding: 0;
      margin: 0;
      // margin-left: 1em;
      list-style: none;

      li {
        margin-bottom: 0.25em;
        margin-left: 1.5em;
        // &::marker {
        //  content: "⛤";
        //   color: transparent;
        //   text-shadow: 0 0 0 var(--secondary);
        // }
        &::before {
          content: "⛤";
          display: inline-block;
          margin-right: 0.5em;
          margin-left: -1.5em;
          text-shadow: 0 0 0 var(--secondary);
        }
      }
    }
  }
</style>
