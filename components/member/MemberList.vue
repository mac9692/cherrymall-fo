<template>
  <div>
    {{ memberList }}
  </div>
</template>

<script>
export default {
  name: "MemberList",

  data() {
    return {
      memberList: {
        memberId: '',
        memberName: '',
        memberAddress: '',
        phoneNumber: '',
      },
    }
  },
  async fetch() {
    try {
      const response = await fetch('/api/member/memberList');
      console.log("response", response);
      this.memberList = response.data;
      console.log("memberList", this.memberList);

    } catch (error) {
      alert(error);
    }
  },
}
</script>

<style scoped>

</style>
