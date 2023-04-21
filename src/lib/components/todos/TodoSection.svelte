<script>
    import Todoinput from "./Todoinput.svelte";
    import { todos } from "../../store/TodoStore";
</script>

<section class="mt-8 space-y-4">
    {#each $todos as todo (todo.id)}
        <Todoinput {todo}/>
    {/each}
</section>