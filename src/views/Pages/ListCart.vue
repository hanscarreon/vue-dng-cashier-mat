<template>
    <div>
    <md-card md-with-hover>
      <md-card-header>
        <div class="md-title">D & G Counter</div>
        <div class="md-subhead">Crew: name in charge</div>
      </md-card-header>

      <md-card-content>
         <div class="md-layout">
        <div class="md-layout-item ">
            <p>Date:10/21/2021</p>
        </div>
         <div class="md-layout-item">
            <p>Order#:647</p>
        </div>
      </div>
        <md-divider></md-divider>
       <md-table>
      <md-table-row>
        <md-table-head >Item</md-table-head>
        <md-table-head>QTY</md-table-head>
        <md-table-head>Price</md-table-head>
        <md-table-head>Total</md-table-head>
      </md-table-row>

      <md-table-row>
        <md-table-cell>Egg pie</md-table-cell>
        <md-table-cell>1</md-table-cell>
        <md-table-cell>120</md-table-cell>
        <md-table-cell>120</md-table-cell>
      </md-table-row>

      <md-table-row>
        <md-table-cell>Cringkles Pack</md-table-cell>
        <md-table-cell>2</md-table-cell>
        <md-table-cell>90</md-table-cell>
        <md-table-cell>180</md-table-cell>
      </md-table-row>

      <md-table-row>
        <md-table-cell>Ube Bar</md-table-cell>
        <md-table-cell>5</md-table-cell>
        <md-table-cell>7</md-table-cell>
        <md-table-cell>35</md-table-cell>
      </md-table-row>
    </md-table>
        <md-divider></md-divider>

      </md-card-content>

      <md-card-actions>
        <md-button>Refresh</md-button>
        <md-button>Check Out</md-button>
      </md-card-actions>
    </md-card>
    </div>
</template>

<script>
export default {
    name:'ListCart'
}
</script>