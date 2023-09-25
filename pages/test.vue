<template>
  <div class="">
    <PerusahaanProfilSubMenu />
    <PerusahaanProfilTabProfile />
    <div>
      <table class="table-auto bg-blue-50 w-full">
        <tr>
          <th>ID</th>
          <th>Username</th>
          <th>Email</th>
          <th>Phone Number</th>
          <th>Edit</th>
          <th>Delete</th>
        </tr>
        <tr v-for="user in submenus" :key="user.id">
          <td>{{ user.id }}</td>
          <td>{{ user.username }}</td>
          <td>{{ user.email }}</td>
          <td>{{ user.mobile }}</td>
          <td>
            <button
              @click="
                showingeditModal = true;
                selectUser(user);
              "
            >
              Edit
            </button>
          </td>
          <td><img :src="user.image" alt="" width="50" height="50" /></td>
        </tr>
      </table>
    </div>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue';

const submenus = ref([]);

// Fungsi untuk mengambil data submenu dari API
async function fetchSubmenus() {
  try {
    const response = await fetch('https://clipan.id/api/users.php?action=read');
    if (!response.ok) {
      throw new Error('Failed to fetch data from the API');
    }
    const data = await response.json();

    // Mengisi submenus dengan data dari API
    submenus.value = data.users; // Mengambil array 'users' dari respon API
  } catch (error) {
    console.error(error);
  }
}

// Panggil fungsi fetchSubmenus saat komponen dimuat
onMounted(fetchSubmenus);
</script>
