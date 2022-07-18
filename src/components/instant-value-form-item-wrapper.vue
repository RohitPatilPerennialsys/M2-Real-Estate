<template>
  <div>
    <form class="form-item">
      <label class="item-title">{{ labeltitle }}</label>
      <select>
        <option disabled hidden selected>{{ labelvalue }}</option>
        <option value="">a</option>
        <option value="">b</option>
      </select>
    </form>
  </div>
</template>

<script>
export default {
  props: ["labeltitle", "labelvalue"],
};
</script>

<style>
.form-item {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  padding-left: 15px;
  margin-top: 20px;
  margin-bottom: 10px;
}
.item-title {
  font-family: Roboto;
  font-size: 18px;
  font-weight: 500;
  font-stretch: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: normal;
  text-align: left;
  color: #fffefe;
}
select,
.select {
  margin-top: 8px;
  width: 310px;
  height: 44px;
}
.select {
  border-top-width: 1px;
  border-left-width: 1px;
  border-bottom-width: 1px;
  border-right-width: 1px;
  padding-right: 0px;
}
</style>
