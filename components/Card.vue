<template>
    <div class="block max-w-sm lg:ml-7 rounded-lg shadow-xl dark:hover:bg-indigo-900 mb-6">
        <img src="https://png.pngtree.com/png-vector/20220803/ourmid/pngtree-office-situation-discussion-vector-illustration-png-image_5720444.png"
            alt="Project Image" class="w-full object-cover mb-4 rounded-md" />
        <div class="px-6 py-4">
            <h4 class="text-xl font-semibold text-white mb-2">Enterprice Resource Planning</h4>
            <p class="text-white mb-2">Business Software</p>
            <CustomIcon text="Automation Tasks" />
            <CustomIcon text="Customer Relation Management" />
            <CustomIcon text="Sales and Marketing" />
            <CustomIcon text="Human Resources (HR)" />
            <CustomIcon text="Supply Chain Management (SCM)" />
        </div>
        <div class="px-6 pt-4 pb-4">
            <span
                class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#nuxt</span>
            <span
                class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#tailwind
                css</span>
            <span
                class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">#bootstrap</span>
        </div>
    </div>
</template>
  

<script>
export default {
    name: "Card"
}
</script>