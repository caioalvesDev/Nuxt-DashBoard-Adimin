<template>
  <section class="grid gap-5 md:grid-cols-2">
    <!-- Revenue -->
    <div class="rounded-lg border bg-card p-6">
      <div class="flex items-center justify-between">
        <p class="text-sm font-medium">Rendimento total</p>
        <span class="shrink-0">
          <Icon name="heroicons:banknotes" class="h-4 w-4 text-muted-foreground" />
        </span>
      </div>

      <p class="mt-1.5 text-xl font-extrabold">R$45,231.89</p>
      <p class="text-xs text-muted-foreground">20% mais do que no mês passado</p>
    </div>
    <!-- Sales -->
    <div class="rounded-lg border bg-card p-6">
      <div class="flex items-center justify-between">
        <p class="text-sm font-medium">Vendas</p>
        <span class="shrink-0">
          <Icon name="heroicons:credit-card" class="h-4 w-4 text-muted-foreground" />
        </span>
      </div>

      <p class="mt-1.5 text-xl font-extrabold">R$12,231</p>
      <p class="text-xs text-muted-foreground">13.2% mais do que no mês passado</p>
    </div>
  </section>
</template>
