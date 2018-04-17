<template>
    <div>
        <h3>Some User Details</h3>
        <p>Loaded user id: {{ $route.params.id }}</p>
        <router-link tag="button" 
            :to="{name: 'userEdit', 
                params: {id: $route.params.id},
                query: { locale: 'en', count: 100 }}"
            class="btn btn-primary">Edit User</router-link>
    </div>
</template>