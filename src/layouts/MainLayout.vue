<template>
  <div class="app-main-layout">
    <nav class="navbar orange lighten-1">
      <div class="nav-wrapper">
        <div class="navbar-left">
          <a href="#">
            <i class="material-icons black-text">dehaze</i>
          </a>
          <span class="black-text">12.12.12</span>
        </div>

        <ul class="right hide-on-small-and-down">
          <li>
            <a
              class="dropdown-trigger black-text"
              href="#"
              data-target="dropdown"
            >
              USER NAME
              <i class="material-icons right">arrow_drop_down</i>
            </a>

            <ul
              id="dropdown"
              class="dropdown-content"
            >
              <li>
                <a
                  href="#"
                  class="black-text"
                >
                  <i class="material-icons">account_circle</i>Profile
                </a>
              </li>
              <li
                class="divider"
                tabindex="-1"
              />
              <li>
                <a
                  href="#"
                  class="black-text"
                >
                  <i class="material-icons">assignment_return</i>Log Out
                </a>
              </li>
            </ul>
          </li>
        </ul>
      </div>
    </nav>

    <ul class="sidenav app-sidenav open">
      <li>
        <a
          href="#"
          class="waves-effect waves-orange pointer"
        >Account</a>
      </li>
      <li>
        <a
          href="#"
          class="waves-effect waves-orange pointer"
        >History</a>
      </li>
      <li>
        <a
          href="#"
          class="waves-effect waves-orange pointer"
        >Planning</a>
      </li>
      <li>
        <a
          href="#"
          class="waves-effect waves-orange pointer"
        >New Record</a>
      </li>
      <li>
        <a
          href="#"
          class="waves-effect waves-orange pointer"
        >Categories</a>
      </li>
    </ul>

    <main class="app-content">
      <router-view />
    </main>

    <div class="fixed-action-btn">
      <a
        class="btn-floating btn-large blue"
        href="#"
      >
        <i class="large material-icons">add</i>
      </a>
    </div>
  </div>
</template>
