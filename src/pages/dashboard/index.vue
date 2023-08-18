<template>
	<div id="app">
		<!--Sidebar with Dimmer -->
		<div class="fixed inset-0 flex z-40">
			<!-- Sidebar -->
			<div
				class="absolute flex top-0 h-screen z-20"
				:class="[right ? 'right-0 flex-row' : 'left-0 flex-row-reverse']"
			>
				<!--toggle button -->
				<!-- <button
					@click.prevent="toggle()"
					class="w-12 h-48 p-1 my-auto rounded text-white bg-gray-600 text-center focus:outline-none hover:bg-gray-500 transition-color duration-300"
				>
					<span
						:class="[right ? '-rotate-90' : 'rotate-90']"
						class="block transform origin-center font-bold"
					>
						Drawer
					</span>
				</button> -->

				<!-- Sidebar Content -->
				<div
					ref="content"
					class="sidebar transition-all duration-700 overflow-hidden flex justify-center"
					:class="[open ? 'max-w-lg' : 'max-w-0']"
				>
					<div class="">
                        <Sidebar />
                    </div>
					<slot></slot>
				</div>
			</div>

			<!-- <transition name="fade"> -->
				<!-- Dimmer -->
				<!-- <div
					v-if="dimmer && open"
					@click="toggle()"
					class="flex-1 bg-gray-400 bg-opacity-75 active:outline-none z-10"
				/>
			</transition> -->
		</div>

		<!-- Page Content -->
		<div
			class="absolute"
		>
			<DashboardContent />
		</div>
	</div>
</template>

<script lang="ts">
    import { defineComponent } from 'vue';
    import Sidebar from './Sidebar.vue';
    import DashboardContent from "./DashboardContent.vue";
    
    export default defineComponent({
        name: 'Dashboard',
        components: {
            // Navbar,
            // Landingpage,
            Sidebar,
            DashboardContent,
            // Footer
        },
        data() {
            return {
                open: true,
                dimmer: false,
                right: false
            };
        },
        methods: {
            toggle() {
                this.open = !this.open;
            }
        }
    });
</script>

<style>
    html {
        background-color: #F9FAFC;
    }
    .fade-enter-active,
    .fade-leave-active {
        transition: opacity 1s ease-out;
    }

    .fade-enter,
    .fade-leave-to {
        opacity: 0;
    }

    .sidebar {
        background-color: #FFFFFF;
        height: 1024px;
        width: 272px;
        box-shadow: 4px 0px 25px 0px #AAAAAA14;
    }
</style>
