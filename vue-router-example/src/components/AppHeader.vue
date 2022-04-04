<template>
  <header id="app-header">
    <nav class="navbar" role="navigation" aria-label="main navigation">
      <div class="navbar-brand">
        <router-link :to="{ name: 'home' }" class="navbar-item">
          <h1>Vue Router Example</h1>
        </router-link>
      </div>

      <div class="navbar-menu">
        <div class="navbar-end">
          <div class="navbar-item">
            <div class="navbar-end">
              <div class="navbar-item">
                <router-link :to="{ name: 'about' }"> About </router-link>
              </div>
            </div>
          </div>
        </div>
      </div>
    </nav>
  </header>
</template>

<style>
#app-header {
  padding: 0 32px;
  background-color: #005eb8;
}

#app-header h1 {
  margin: 0;
  font-weight: 700;
  font-size: 1.5rem;
  color: #fff;
}

#app-header nav {
  background-color: #005eb8;
}

#app-header nav .navbar-item a {
  color: #fff;
  text-transform: uppercase;
}
</style>
