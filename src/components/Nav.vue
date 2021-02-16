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
        title: 'Main Navigation',
        // hidden: false
        hiddenOnCollapse: true,
        // class: ''
        // attributes: {}
    },
      				{
			          href: '/',
			          title: 'Installation',
			          icon: 'fa fa-download',
			          badge: {
					            text: 'new',
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
	

</style>