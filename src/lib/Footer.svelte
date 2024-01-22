<script lang="ts">
  const socialLinks: { title: string, url: string}[] = [
    {
      title: "Github",
      url: "https://github.com/bradstemke",
    },
    {
      title: "Instagram",
      url: "http://instagram.com/bradstemke",
    },
    {
      title: "Twitter",
      url: "https://twitter.com/bradstemke",
    }
  ];
</script>

<footer>
  <div class="inner">
    <div class="linklist-wrapper">
      <ul>
        {#each socialLinks as link}
          <li>
            <a href={link.url} target="_blank">{link.title}</a>
          </li>
        {/each }
      </ul>  
    </div>

    <div class="copyright">
      <p>©{new Date().getFullYear()}</p>
    </div>
  </div>
</footer>

<style lang="css">

footer {
  display: flex;
  flex-direction: column;
  background-color: var(--color-primary-tan);
}

@media only screen and (min-width: 900px) {
  footer {
    flex-direction: row;
    padding: var(--spacing-3);
  }
}

.inner {
  display: flex;
  align-items: center;
  flex-direction: column;
  padding: var(--spacing-2) var(--spacing-2) var(--spacing-4);
}

@media only screen and (min-width: 900px) {
  .inner {
    flex-direction: row;
    width: 100%;
    padding: var(--spacing-2) var(--spacing-3);
  }
}

.copyright {
  text-align: center;
  display: flex;
  flex: 1;
  justify-content: center;
  align-items: center;
}

@media only screen and (min-width: 900px) {
  .copyright {
    justify-content: flex-end;
  }
}

.linklist-wrapper {
  display: flex;
  flex: 1;
  justify-content: center;
  align-content: center;
  margin: 0 0 var(--spacing-4) 0;
}

@media only screen and (min-width: 900px) {
  .linklist-wrapper {
    justify-content: flex-start;
    margin: 0;
  }
}

ul li {
  display: inline-block;    
  background-color: var(--color-primary-green);
  margin-right: var(--spacing-2);
}

@media only screen and (min-width: 900px) {
  ul li {
    margin-right: var(--spacing-1);
  }
}

ul li:last-of-type {
  margin-right: 0;
}

ul li:focus, ul li:hover, ul li:focus-visible {
  transform: rotateZ(6deg);
  outline-color: var(--color-primary-yellow);
}

ul li:nth-of-type(even):focus, ul li:nth-of-type(even):hover, ul li:nth-of-type(even):focus-visible {
  transform: rotateZ(-6deg);
}

ul li a {
  display: block;
  color: var(--color-primary-white);
  text-decoration: none;
  text-transform: uppercase;
  padding: var(--spacing-1);
}

</style>