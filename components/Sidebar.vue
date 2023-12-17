<template>
  <aside class="sticky top-[65px] h-[calc(100vh-65px)] py-5">
    <div
      class="flex h-full w-full flex-col gap-5 overflow-y-auto rounded-md border bg-card pb-5 scrollbar-thin scrollbar-thumb-input scrollbar-thumb-rounded-md"
    >
      <SidebarItem :links="menu" />

      <div class="mt-auto">
        <SidebarItem :links="bottomMenu" />
      </div>
    </div>
  </aside>
</template>

<script setup lang="ts">
    const bottomMenu = [
      {
        title: "Configurações",
        icon: "heroicons:cog-8-tooth",
      },
      {
        title: "Ajuda",
        icon: "heroicons:question-mark-circle",
      },
      {
        title: "Logout",
        icon: "heroicons:arrow-left-on-rectangle",
      },
    ];
    const menu = [
      {
        title: "Dashboard",
        icon: "heroicons:home",
      },
      {
        title: "Clientes",
        icon: "heroicons:user-group",
        items: [
          { title: "Lista" },
          { title: "Criar" },
          { title: "Editar" },
          { title: "Deletar" },
          { title: "Detalhes" },
        ],
      },
      {
        title: "Pedidos",
        icon: "heroicons:shopping-cart",
        items: [
          { title: "Lista" },
          { title: "Criar" },
          { title: "Editar" },
          { title: "Deletar" },
          { title: "Detalhes" },
        ],
      },
      {
        title: "Produtos",
        icon: "heroicons:cube",
        items: [
          { title: "Lista" },
          { title: "Criar" },
          { title: "Editar" },
          { title: "Deletar" },
          { title: "Detalhes" },
        ],
      },
      {
        title: "Funcionários",
        icon: "heroicons:user",
        items: [
          { title: "Lista" },
          { title: "Criar" },
          { title: "Editar" },
          { title: "Deletar" },
          { title: "Detalhes" },
        ],
      },
      {
        title: "Análise",
        icon: "heroicons:chart-pie",
        items: [{ title: "Visão geral" }, { title: "Estatisticas" }, { title: "Tendências" }],
      },
    ];
</script>
