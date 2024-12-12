<script>
import AuthenticatedLayout from "@/Layouts/AuthenticatedLayout.vue";
import {Head} from "@inertiajs/vue3";

export default {
    name: "Index",
    components: {Head, AuthenticatedLayout}
}
</script>

<template>
    <Head title="Tickets" />

    <AuthenticatedLayout>
        <template #header>
            <h2
                class="text-xl font-semibold leading-tight text-gray-800"
            >
                Tickets
            </h2>
        </template>

        <div class="py-12">
            <div class="mx-auto max-w-7xl sm:px-6 lg:px-8">
                <div
                    class="overflow-hidden bg-white shadow-sm sm:rounded-lg"
                >
                    <div class="p-6 text-gray-900">
                        <div class="flex gap-6">
                            <!-- Sidebar Categories -->
                            <aside class="w-1/4 bg-white shadow rounded p-4 space-y-4">
                                <button class="w-full text-left px-4 py-2 bg-blue-500 text-white rounded hover:bg-blue-600">Category 1</button>
                                <button class="w-full text-left px-4 py-2 bg-gray-200 rounded hover:bg-gray-300">Category 2</button>
                                <button class="w-full text-left px-4 py-2 bg-gray-200 rounded hover:bg-gray-300">Category 3</button>
                                <button class="w-full text-left px-4 py-2 bg-gray-200 rounded hover:bg-gray-300">Category 4</button>
                            </aside>

                            <!-- Main Content -->
                            <main class="w-3/4 space-y-4">
                                <!-- Filters and Export -->
                                <div class="flex items-center justify-between">
                                    <div class="flex gap-4">
                                        <select class="px-4 py-2 border border-gray-300 rounded">
                                            <option>Status</option>
                                            <option>Status 1</option>
                                            <option>Status 2</option>
                                        </select>

                                        <select class="px-4 py-2 border border-gray-300 rounded">
                                            <option>Filter</option>
                                            <option>Filter 1</option>
                                            <option>Filter 2</option>
                                        </select>
                                    </div>

                                    <button class="px-4 py-2 bg-blue-500 text-white rounded hover:bg-blue-600">Export</button>
                                </div>
                                <!-- Item Counter -->
                                <div class="text-gray-500">143 items</div>

                                <!-- FAQ Items -->
                                <div class="space-y-4">
                                    <div class="p-4 bg-white shadow-md rounded">
                                        <h3 class="font-bold text-lg">That is a question?</h3>
                                        <p class="text-gray-600">This is answer</p>
                                    </div>

                                    <div class="p-4 bg-white shadow-md rounded">
                                        <h3 class="font-bold text-lg">That is a question?</h3>
                                        <p class="text-gray-600">This is answer</p>
                                    </div>

                                    <div class="p-4 bg-white shadow-md rounded">
                                        <h3 class="font-bold text-lg">That is a question?</h3>
                                        <p class="text-gray-600">This is answer</p>
                                    </div>

                                    <div class="p-4 bg-white shadow-md rounded">
                                        <h3 class="font-bold text-lg">That is a question?</h3>
                                        <p class="text-gray-600">This is answer</p>
                                    </div>
                                </div>
                            </main>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </AuthenticatedLayout>
</template>

<style scoped>

</style>
