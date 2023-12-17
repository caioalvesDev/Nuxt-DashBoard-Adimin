<template>
  <div class="sticky top-20 mt-5">
    <p class="font-bold">Lembretes</p>

    <ul>
      <template v-for="(r, i) in reminders" :key="i">
        <li>
          <div class="mt-5 flex items-center justify-between">
            <div class="flex items-center gap-3">
              <Icon name="heroicons:check-circle" class="h-4 w-4 text-muted-foreground" />
              <span class="text-sm">{{ r.title }}</span>
            </div>
            <span class="text-sm text-muted-foreground">{{ r.time }}</span>
          </div>
        </li>
      </template>
    </ul>
  </div>
</template>

<script setup lang="ts">
    const reminders = [
      { title: "Ligue para João", time: "10:00 AM" },
      { title: "Encontro com Maria", time: "11:00 AM" },
      { title: "Ligue para Sally", time: "12:00 PM" },
      { title: "Almoço com Sara", time: "1:00 PM" },
    ];
</script>
