
import Me_movie from '~/components/Me_movie.vue';
<template>
    <IonPage>
        <IonContent class="ion-padding">
          <IonButton> Logout </IonButton>
            <Profile />
            <Ioncard>
              <Me_coupon />
            </Ioncard>

            <van-row class="user-links">
      <van-col span="6">
        <van-icon name="pending-payment" />
        
        待付款
      </van-col>
      <van-col span="6">
        <van-icon name="records" />
        待接单
      </van-col>
      <van-col span="6">
        <van-icon name="tosend" />
        待发货
      </van-col>
      <van-col span="6">
        <van-icon name="logistics" />
        已发货
      </van-col>
    </van-row>
    <Me_movie />
        </IonContent>
    
        <Tabbar2 />
        <Clearpage />
    </IonPage>


</template>

<style lang="less">
body {
  margin: 0;
  font-size: 16px;
  background-color: #f8f8f8;
  -webkit-font-smoothing: antialiased;
}

.user {
  &-poster {
    width: 100%;
    height: 53vw;
    display: block;
  }

  &-group {
    margin-bottom: 15px;
  }

  &-links {
    padding: 15px 0;
    font-size: 12px;
    text-align: center;
    background-color: #fff;

    .van-icon {
      display: block;
      font-size: 24px;
    }
  }
}
</style>
