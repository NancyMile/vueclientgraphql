<script>
import TASKS_QUERY from '@/graphql/Tasks.gql';

export default{
    data() {
        return {
            tasks: null,
        };
    },
    apollo: {
        tasks: TASKS_QUERY,
    },
};  
</script>

<template>
    <div>
        <ul>
            <li v-for="task in tasks" :key="task.id">
                {{ task.task }}
            </li>
        </ul>
    </div>
</template>