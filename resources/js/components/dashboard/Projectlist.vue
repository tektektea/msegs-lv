<template>
 <main class="flex-1 overflow-x-hidden overflow-y-auto bg-gray-200">
                <div class="container mx-auto px-6 py-8">
                    <h3 class="text-gray-700 text-3xl font-medium">Dashboard</h3>
    
                    <div class="mt-4">
                        <div class="flex flex-wrap -mx-6">
                            <div class="w-full px-6 sm:w-1/2 xl:w-1/3">
                                <div class="flex items-center px-5 py-6 shadow-sm rounded-md bg-white">
                                    <div class="p-3 rounded-full bg-indigo-600 bg-opacity-75" style="color:white">
                                       <i class="fas fa-project-diagram px-2"></i>
                                    </div>
    
                                    <div class="mx-5">
                                        <h4 class="text-2xl font-semibold text-gray-700">{{projects.length}}</h4>
                                        <div class="text-gray-500">Projects Added</div>
                                    </div>
                                </div>
                            </div>
                             <span class="flex items-center px-5 py-6 shadow-sm rounded-md bg-white">
                        <router-link :to="{name: 'addproject'}" class="text-indigo-600 hover:text-indigo-900 font-bold">Add Project</router-link>

                            </span>
<!--     
                            <div class="w-full mt-6 px-6 sm:w-1/2 xl:w-1/3 sm:mt-0">
                                <div class="flex items-center px-5 py-6 shadow-sm rounded-md bg-white">
                                    <div class="p-3 rounded-full bg-orange-600 bg-opacity-75">
                                        <svg class="h-8 w-8 text-white" viewBox="0 0 28 28" fill="none"
                                            xmlns="http://www.w3.org/2000/svg">
                                            <path
                                                d="M4.19999 1.4C3.4268 1.4 2.79999 2.02681 2.79999 2.8C2.79999 3.57319 3.4268 4.2 4.19999 4.2H5.9069L6.33468 5.91114C6.33917 5.93092 6.34409 5.95055 6.34941 5.97001L8.24953 13.5705L6.99992 14.8201C5.23602 16.584 6.48528 19.6 8.97981 19.6H21C21.7731 19.6 22.4 18.9732 22.4 18.2C22.4 17.4268 21.7731 16.8 21 16.8H8.97983L10.3798 15.4H19.6C20.1303 15.4 20.615 15.1004 20.8521 14.6261L25.0521 6.22609C25.2691 5.79212 25.246 5.27673 24.991 4.86398C24.7357 4.45123 24.2852 4.2 23.8 4.2H8.79308L8.35818 2.46044C8.20238 1.83722 7.64241 1.4 6.99999 1.4H4.19999Z"
                                                fill="currentColor"></path>
                                            <path
                                                d="M22.4 23.1C22.4 24.2598 21.4598 25.2 20.3 25.2C19.1403 25.2 18.2 24.2598 18.2 23.1C18.2 21.9402 19.1403 21 20.3 21C21.4598 21 22.4 21.9402 22.4 23.1Z"
                                                fill="currentColor"></path>
                                            <path
                                                d="M9.1 25.2C10.2598 25.2 11.2 24.2598 11.2 23.1C11.2 21.9402 10.2598 21 9.1 21C7.9402 21 7 21.9402 7 23.1C7 24.2598 7.9402 25.2 9.1 25.2Z"
                                                fill="currentColor"></path>
                                        </svg>
                                    </div>
    
                                    <div class="mx-5">
                                        <h4 class="text-2xl font-semibold text-gray-700">20</h4>
                                        <div class="text-gray-500">Incomplete</div>
                                    </div>
                                </div>
                            </div>
    
                            <div class="w-full mt-6 px-6 sm:w-1/2 xl:w-1/3 xl:mt-0">
                                <div class="flex items-center px-5 py-6 shadow-sm rounded-md bg-white">
                                    <div class="p-3 rounded-full bg-pink-600 bg-opacity-75">
                                        <svg class="h-8 w-8 text-white" viewBox="0 0 28 28" fill="none"
                                            xmlns="http://www.w3.org/2000/svg">
                                            <path d="M6.99998 11.2H21L22.4 23.8H5.59998L6.99998 11.2Z" fill="currentColor"
                                                stroke="currentColor" stroke-width="2" stroke-linejoin="round"></path>
                                            <path
                                                d="M9.79999 8.4C9.79999 6.08041 11.6804 4.2 14 4.2C16.3196 4.2 18.2 6.08041 18.2 8.4V12.6C18.2 14.9197 16.3196 16.8 14 16.8C11.6804 16.8 9.79999 14.9197 9.79999 12.6V8.4Z"
                                                stroke="currentColor" stroke-width="2"></path>
                                        </svg>
                                    </div>
    
                                    <div class="mx-5">
                                        <h4 class="text-2xl font-semibold text-gray-700">21</h4>
                                        <div class="text-gray-500">Enquiries</div>
                                    </div>
                                </div>
                            </div> -->
                        </div>
                    </div>
    
                    <div class="mt-8">
    
                    </div>
    


    <!-- tables -->
                    <div class="flex flex-col mt-8">
                        <div class="-my-2 py-2 overflow-x-auto sm:-mx-6 sm:px-6 lg:-mx-8 lg:px-8">
                            <div
                                class="align-middle inline-block min-w-full shadow overflow-hidden sm:rounded-lg border-b border-gray-200">
                                <table class="min-w-full">
                                    <thead>
                                        <tr>
                                            <th
                                                class="px-6 py-3 border-b border-gray-200 bg-gray-50 text-left text-xs leading-4 font-medium text-gray-500 uppercase tracking-wider">
                                                Project</th>
                                            <th
                                                class="px-6 py-3 border-b border-gray-200 bg-gray-50 text-left text-xs leading-4 font-medium text-gray-500 uppercase tracking-wider">
                                                Date/Sub-title</th>
                                            <th
                                                class="px-6 py-3 border-b border-gray-200 bg-gray-50 text-left text-xs leading-4 font-medium text-gray-500 uppercase tracking-wider">
                                                Status</th>
                                            <th
                                                class="px-6 py-3 border-b border-gray-200 bg-gray-50 text-left text-xs leading-4 font-medium text-gray-500 uppercase tracking-wider">
                                                Action</th>
                                            <!-- <th class="px-6 py-3 border-b border-gray-200 bg-gray-50">
                        <router-link :to="{name: 'addproject'}" class="text-indigo-600 hover:text-indigo-900 font-bold">Add Project</router-link>


                                            </th> -->
                                        </tr>
                                    </thead>
    
                                    <tbody class="bg-white" v-for="project in projects" :key="project.id">
                                        <tr>
                                            <td class="px-6 py-4 whitespace-no-wrap border-b border-gray-200">
                                                <div class="flex items-center">
                                                    <div class="flex-shrink-0 h-10 w-10">
                                                        <img class="h-10 w-10 rounded-full"
                                                        src="../../assets/webapp.png"
                                                            alt="">
                                                    </div>
    
                                                    <div class="ml-4">
                                                        <div class="text-sm leading-5 font-medium text-gray-900">{{ project.title }}
                                                        </div>
                                                        <div class="text-sm leading-5 text-gray-500">{{ project.id}}</div>
                                                    </div>
                                                </div>
                                            </td>
    
                                            <td class="px-6 py-4 whitespace-no-wrap border-b border-gray-200">
                                                <div class="text-sm leading-5 text-gray-900">{{ project.date}}</div>
                                                <div class="text-sm leading-5 text-gray-500">{{project.subtitle}}</div>
                                            </td>
    
                                            <td class="px-6 py-4 whitespace-no-wrap border-b border-gray-200">
                                                <span
                                                    class="px-2 inline-flex text-xs leading-5 font-semibold rounded-full bg-green-100 text-green-800">Active</span>
                                            </td>
    
                                            <!-- <td
                                                class="px-6 py-4 whitespace-no-wrap border-b border-gray-200 text-sm leading-5 text-gray-500">
                                                </td> -->
    
                                            <td
                                                class="px-6 py-4 whitespace-no-wrap text-right border-b border-gray-200 text-sm leading-5 font-medium">
                                               
                        <router-link :to="{name: 'projectsupdate', params: { id: project.id },}" class="text-indigo-600 hover:text-indigo-900 font-bold">Edit</router-link>
                                    <button class="text-red-600  " @click="deleteProduct(project.id)">Delete </button>
                                            </td>
                                        </tr>
                                       
                                    </tbody>
                                </table>
                            </div>
                        </div>
                    </div>
                </div>
            </main>
</template>

<script>
export default {
	data(){
		return{
			user:null,
            projects:[]
		}
	},
 created() {
        this.axios.get("/api/projects/").then((response) => {
            console.log(response.data);
            this.projects = response.data;
        });
    },
    methods:{
         deleteProduct(id) {
            this.axios.delete(`api/projects/${id}`).then((response) => {
                let i = this.projects.map((data) => data.id).indexOf(id);
                this.projects.splice(i, 1);
            });
        },
    }
}
</script>

<style>

</style>