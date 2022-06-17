<template>
    <div class="contacts">
        <h3>CONTACT INFORMATION</h3>
        <hr>
        <ul>
            <li><i class="fa-solid fa-location-dot"></i>{{ contact.address }}</li>
            <li><i class="fa-solid fa-phone-flip"></i>{{ contact.phoneNumber }}</li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'ContactInformation',
    data() {
        return {
            contact: {
                address: "121 King Street, London United Kingdom",
                phoneNumber: "1.800.458.556"
            }
        }
    }
}
</script>

<style lang="scss" scoped>
ul {
    list-style-type: none;

    li{
        margin-bottom: 10px;

       
    }
}

hr {
    margin:20px 0;
    width: 50px;
    background-color: var(--primary-color);
    border-color: var(--primary-color);
}

.contacts {

    & svg {
        margin-right: 10px;
        color: var(--primary-color);

        
    }
}
</style>