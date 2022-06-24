<script lang="ts">
  import Icon from '@iconify/svelte';
</script>

<div class="navbar sticky top-0 z-40 bg-base-300 shadow-xl rounded-box">
  <div class="flex-1 gap-5">
    <button class="btn btn-circle btn-ghost normal-case text-xl">
      <Icon icon="fe:bar" width="35" />
    </button>
    <h1 class="pr-10">Demo app</h1>
    <div class="form-control hidden sm:block">
      <div class="input-group">
        <input type="text" placeholder="Search" class="input input-bordered w-60" />
        <button class="btn btn-square">
          <Icon icon="fe:search" width="24" />
        </button>
      </div>
    </div>
  </div>
  <div class="flex-none gap-2">
    <div class="dropdown dropdown-end">
      <!-- tabindex here is used to trigger the menu -->
      <div tabindex="0" class="btn btn-ghost btn-circle avatar">
        <div class="w-10 rounded-full">
          <img src="https://api.lorem.space/image/face?hash=33791" alt="user" />
        </div>
      </div>
      <ul tabindex="0" class="mt-3 p-2 shadow menu menu-compact dropdown-content bg-base-100 rounded-box w-52">
        <li>
          <a class="justify-between" href="/">
            Profile
            <span class="badge">New</span>
          </a>
        </li>
        <li><a href="/settings">Settings</a></li>
        <li><a href="/logout">Logout</a></li>
      </ul>
    </div>
  </div>
</div>