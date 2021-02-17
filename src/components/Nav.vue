<template>
	<div>
 <sidebar-menu :menu="menu" :collapsed="collapsed"/>
 </div>
</template>

<script>
	export default {
		data () {
    		return {
      			menu: [
      			{
        header: true,
        title: 'Главное меню',
        // hidden: false
        hiddenOnCollapse: true,
        // class: ''
        attributes: {'style':'height: 50px;',}
    },
      				{
			          href: '/',
			          title: 'Installation',
			          icon: 'fa fa-download',
			          badge: {
					            text: '+15',
					            class: 'vsm--badge_default',
					            // attributes: {}
					            element: 'span'
					        }
			        },
			        {
			          href: '/basic-usage',
			          title: 'Basic Usage',
			          icon: 'fa fa-code'
			        },

      			],
      			collapsed: true,
      		}
      	}
	}	
</script>

<style scoped>

	.v-sidebar-menu {
		top: 50px;
		color: 
	}

	.v-sidebar-menu .vsm--link.vsm--link_active {
		color: red;
	}

	

	
	

</style>