<script>
import SidebarItem from '@/components/SidebarItem.vue';

export default {
   data() {
      return {
         homeElements: [
            { id: 'dashboard', title: 'Dashboard', icon: 'pi-home' },
            { id: 'team', title: 'Team', icon: 'pi-users' },
            { id: 'messages', title: 'Messages', icon: 'pi-inbox' },
            { id: 'calendar', title: 'Calendar', icon: 'pi-calendar' },
            { id: 'reports', title: 'Reports', icon: 'pi-file' }
         ],
         departments: [
            { id: 'alldepartments', title: 'All Departments', icon: 'pi-sitemap' },
            { id: 'artistbookings', title: 'Artist Bookings', icon: 'pi-headphones' },
            { id: 'gastronomy', title: 'Gastronomy', icon: 'pi-shop' },
            { id: 'legalSecurityControl', title: 'Legal, Security & Control', icon: 'pi-shield' },
            { id: 'marketing', title: 'Marketing & Sponsors', icon: 'pi-volume-up' },
            { id: 'ticketing', title: 'Ticketing and Pre-sale ', icon: 'pi-receipt' },
            { id: 'stageEquipment', title: 'Stage & Equipment', icon: 'pi-sliders-v' }
         ]
      };
   },
   
   components: {
      SidebarItem
   }
};

</script>

<template>
   <div class="sidebar-items">
      <h3>Home</h3>
      <SidebarItem v-for="element in homeElements" :title="element.title" :icon="element.icon" />
      <h3>Organization</h3>
      <SidebarItem v-for="department in departments" :title="department.title" :icon="department.icon" />
   </div>
</template>

<style scoped>

.sidebar-items {
   display: flex;
   flex-direction: column;
   align-items: left;
   padding: 10px 0;
   box-shadow: 0px 2px 10px 0px rgba(0,0,0,0.1);
}

.sidebar-items h3 {
   margin: 0 0 0 20px;
   padding: 10px 0;
   /* border-bottom: 1px solid #e0e0e0; */
}
</style>