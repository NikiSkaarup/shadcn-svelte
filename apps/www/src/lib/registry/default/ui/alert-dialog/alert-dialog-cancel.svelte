<script lang="ts">
	import { AlertDialog as AlertDialogPrimitive } from "bits-ui";
	import { buttonVariants } from "@/registry/default/ui/button";
	import { cn } from "$lib/utils";

	type $$Props = AlertDialogPrimitive.CancelProps;

	let className: $$Props["class"] = undefined;
	export { className as class };
</script>

<AlertDialogPrimitive.Cancel
	class={cn(
		buttonVariants({ variant: "outline" }),
		"mt-2 sm:mt-0",
		className
	)}
	{...$$restProps}
>
	<slot />
</AlertDialogPrimitive.Cancel>
