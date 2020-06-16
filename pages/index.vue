<template>
  <div>
    <links></links>
    <h1 class="h1-responsive">Ultimas Noticias</h1>
    <hr />
    <mdb-card-group column>
      <template v-for="noti in noticias.data">
        <mdb-card sm="4" v-if="noti.full_picture" :key="noti.created_time" wide>
          <mdb-view hover cascade>
            <a to="#!">
              <mdb-card-image :src="noti.full_picture"></mdb-card-image>
              <mdb-mask flex-center waves overlay="white-slight"></mdb-mask>
            </a>
          </mdb-view>
          <mdb-card-body class="text-center" cascade>
            <mdb-card-text>{{ noti.message }}</mdb-card-text>
          </mdb-card-body>
        </mdb-card>
      </template>
    </mdb-card-group>
  </div>
</template>

<script>
const moment = require("moment");
import axios from "axios";
import links from "../components/Links";
import {
  mdbContainer,
  mdbRow,
  mdbCol,
  mdbCard,
  mdbCardImage,
  mdbCardHeader,
  mdbCardBody,
  mdbCardTitle,
  mdbCardText,
  mdbCardFooter,
  mdbCardUp,
  mdbCardAvatar,
  mdbCardGroup,
  mdbBtn,
  mdbView,
  mdbMask,
  mdbIcon,
} from "mdbvue";

export default {
  layout: "inicio",
  components: {
    mdbContainer,
    mdbRow,
    mdbCol,
    mdbCard,
    mdbCardImage,
    mdbCardHeader,
    mdbCardBody,
    mdbCardTitle,
    mdbCardText,
    mdbCardFooter,
    mdbCardUp,
    mdbCardAvatar,
    mdbCardGroup,
    mdbBtn,
    mdbView,
    mdbMask,
    mdbIcon,
    links,
  },

  data() {
    return {
      noticias: {},
    };
  },
  filters: {
    fecha: function(value) {
      return moment(value).format("DD/MM/YYYY");
    },
  },
  mounted: function() {
    console.log(process.env.GOOGLE_PHOTOS_KEY);
    this.getDatosFb();
  },
  methods: {
    getDatosFb() {
      //http://meanandroid.com/latestposts/how-never-expiring-facebook-access-token/
      var self = this;
      this.$axios
        .get("https://graph.facebook.com/v3.3/distrito5zona9saac/feed", {
          params: {
            access_token:
              "EAAJSo7qsf6oBAHZC8D8BWLYP1epHDRulhA0YgPcgCZAvZBiwcX1fdLxmKZBbuALnXqXm9Pw9VZAOTBZBhTuXB0aLZBKea2AkhZBkj2VN4KaZCQZCqfwZBRTLOuJ51F3Kz1LbaUXraiiQAaA5r4ckP1WCc1Px6JE4ZBMmXxBSCP6FYMXzRwZDZD",
            fields:
              "created_time,full_picture,message,story,permalink_url,shares,via,comments,picture,sharedposts",
            //fields: 'created_time,event,expanded_width,expanded_height,feed_targeting,from,full_picture,height,icon,id,message,message_tags,parent_id,picture,place,privacy,promotable_id,promotion_status,properties,scheduled_publish_time,shares,story,story_tags,subscribed,target,targeting,timeline_visibility,updated_time,via,video_buying_eligibility,width,comments{application,attachment,can_comment,can_like,can_remove,can_reply_privately,comment_count,created_time,from,id,is_private,like_count,live_broadcast_timestamp,message,message_tags,object,parent,permalink_url,private_reply_conversation,user_likes,is_hidden,comments},permalink_url',
            limit: 10,
            transport: "cors",
          },
        })
        .then(function(response) {
          self.noticias = response.data;
          //console.log(response);
        });
    },
  },
};
</script>
