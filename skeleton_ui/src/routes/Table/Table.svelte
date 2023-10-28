<script>
	import Row from './Row.svelte';
	import { popup } from '@skeletonlabs/skeleton';
	
	let comboboxValue = "";

	const popupCombobox = {
		event: 'focus-click',
		target: 'popupCombobox',
		placement: 'bottom',
		closeQuery: '.listbox-item'
	};
				
</script>

<div class="table-container">
	<!-- Native Table Element -->
	<table class="table table-hover table-compact">
		<thead>
			<tr>
				<th>
					
				</th>
				<th>Ladle ID</th>
				<th>Status</th>
				<th>Entry Time</th>
				<th>Exit Time</th>
				<th>Heat Cycles</th>
			</tr>
		</thead>
		<tbody>
			<Row />
		</tbody>
	</table>
</div>
