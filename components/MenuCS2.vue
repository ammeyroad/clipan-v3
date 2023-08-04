<template>
  <div class="text-right">
    <Menu as="div" class="relative text-right">
      <div>
        <MenuButton
          class="bg-gray-100 hover:bg-blue-400 font-medium rounded-xl text-sm p-1.5 text-center inline-flex items-center text-blue-500 hover:text-white"
        >
           <Icon name="solar:call-chat-rounded-bold-duotone" class="w-8 h-8" />
         
        </MenuButton>
      </div>

      <transition
        enter-active-class="transition duration-100 ease-out"
        enter-from-class="transform scale-95 opacity-0"
        enter-to-class="transform scale-100 opacity-100"
        leave-active-class="transition duration-75 ease-in"
        leave-from-class="transform scale-100 opacity-100"
        leave-to-class="transform scale-95 opacity-0"
      >
        <MenuItems
          class="absolute right-0 mt-4 w-56 origin-top-right divide-y divide-gray-100 rounded-md bg-white shadow-lg ring-1 ring-black ring-opacity-5 focus:outline-none"
        >
          <div class="px-1 py-1">
            <MenuItem v-slot="{ active }">
              <button
                :class="[
                  active ? 'bg-blue-600 text-white' : 'text-gray-900',
                  'group flex w-full items-center rounded-md px-2 py-2 text-sm',
                ]"
              >
                <EditIcon
                  :active="active"
                  class="mr-2 h-5 w-5 text-blue-600"
                  aria-hidden="true"
                />
                Edit
              </button>
            </MenuItem>
            <MenuItem v-slot="{ active }">
              <button
                :class="[
                  active ? 'bg-blue-600 text-white' : 'text-gray-900',
                  'group flex w-full items-center rounded-md px-2 py-2 text-sm',
                ]"
              >
                <DuplicateIcon
                  :active="active"
                  class="mr-2 h-5 w-5 text-blue-600"
                  aria-hidden="true"
                />
                Duplicate
              </button>
            </MenuItem>
          </div>
          <div class="px-1 py-1">
            <MenuItem v-slot="{ active }">
              <button
                :class="[
                  active ? 'bg-blue-600 text-white' : 'text-gray-900',
                  'group flex w-full items-center rounded-md px-2 py-2 text-sm',
                ]"
              >
                <ArchiveIcon
                  :active="active"
                  class="mr-2 h-5 w-5 text-blue-600"
                  aria-hidden="true"
                />
                Archive
              </button>
            </MenuItem>
            <MenuItem v-slot="{ active }">
              <button
                :class="[
                  active ? 'bg-blue-600 text-white' : 'text-gray-900',
                  'group flex w-full items-center rounded-md px-2 py-2 text-sm',
                ]"
              >
                <MoveIcon
                  :active="active"
                  class="mr-2 h-5 w-5 text-blue-600"
                  aria-hidden="true"
                />
                Move
              </button>
            </MenuItem>
          </div>

          <div class="px-1 py-1">
            <MenuItem v-slot="{ active }">
              <button
                :class="[
                  active ? 'bg-blue-600 text-white' : 'text-gray-900',
                  'group flex w-full items-center rounded-md px-2 py-2 text-sm',
                ]"
              >
                <DeleteIcon
                  :active="active"
                  class="mr-2 h-5 w-5 text-blue-600"
                  aria-hidden="true"
                />
                Delete
              </button>
            </MenuItem>
          </div>
        </MenuItems>
      </transition>
    </Menu>
  </div>
</template>

<script setup>
import { Menu, MenuButton, MenuItems, MenuItem } from '@headlessui/vue'

</script>
