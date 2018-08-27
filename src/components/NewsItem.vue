<template>
	<div class="w-full rounded-lg h-48 border border-grey-light mt-6 flex">
		
		<div class="w-1/4 h-48 overflow-hidden bg-cover rounded-l-lg" :style="'background-image: url('+ item.urlToImage +')'">
			<!-- <img :src="item.urlToImage" :alt="item.title" class=""> -->
		</div>
	
		<div class="w-3/4 pl-2 pr-2">

			<div class="text-black font-bold text-l mb-4 mt-2"><a class="no-underline text-black hover:underline" :href="item.url" target="_blank">{{item.title}}</a></div>

			<div class="h-24">
				<p class="text-xs text-grey-darker">
					{{ item.description }}
				</p>
			</div>

			<div class="flex text-xs mt-4 justify-between items-baseline text-grey-darker">
				<div class="w-1/2">{{ item.author }}</div>
				<div class="w-1/2 text-right">{{ item.publishedAt | to_date }}</div>
			</div>

		</div>
	</div>
</template>

<script>

import moment from 'moment'

export default {

  name: 'news-item',

  props: ['item'],

  data () {
    return {

    }
  },

  filters: {
  	to_date(timestamp) {
  		return moment(timestamp).format('Do MMM YYYY, h:mm a')
  	}
  }
}
</script>

<style lang="css" scoped>
</style>