# APIs-Facebook-no-cookie-token
API lấy data facebook không cần dùng cookie hay token
HOÀN TOÀN MIỄN PHÍ

<details>

<summary>Get reactions (cảm xúc) của bài viết</summary>


```http
GET http://graph.scanfb.top/graphql?action=post_reactions&post_id=7523377607684413&cursor=&access_token=N8o3eySfREuw1pbt3fmcLg
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `access_token` | `string` | **Bắt buộc**. Token trên được chia sẽ công khai, nhiều người dùng, request có thể sẽ chậm. Liên hệ Kiệt để nhận Token riêng miễn phí |
| `post_id` | `string` | **Bắt buộc**. ID bài viết, dạng số, không có dấu _ |
| `cursor` | `string` |  Request đầu tiên có thể để trống, lấy trong response truyền vào cho request tiếp theo |


### Response
```json
{
    "success": true,
    "message": "",
    "data": {
        "data": {
            "node": {
                "__typename": "Feedback",
                "reactors": {
                    "edges": [
                        {
                            "feedback_reaction_info": {
                                "face_image": {
                                    "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An_EjZkxLL70Wj-QVF5bQc6a1UbfBdeaindMayM5EB_nn6ZbIDF4U4rIKO9ISgyJppdBzZM3T20shDptNixRsCGCU8YNtZNKquX5opCN3SYVdwkNT9uoGFDh8UtV4G0.png?ccb=10-5&oh=00_AfDV4r7igtXZ0tBv7FMWxrMmqWEB0sC4g9L6LC7fpdeEHg&oe=664456F5&_nc_sid=7da55a"
                                },
                                "id": "1635855486666999"
                            },
                            "node": {
                                "id": "100010809121296",
                                "__typename": "User",
                                "__isActor": "User",
                                "mutual_friends": {
                                    "count": 0
                                },
                                "__isProfile": "User",
                                "can_viewer_message": true,
                                "friendship_status": "CAN_REQUEST",
                                "subscribe_status": "CAN_SUBSCRIBE",
                                "secondary_subscribe_status": "REGULAR_FOLLOW",
                                "invite_status_in_feedback": "NOT_INVITABLE",
                                "follower_invite_status_in_feedback": "NOT_INVITABLE",
                                "name": "Nguyễn Đình Dũng",
                                "__isEntity": "User",
                                "profile_url": "https://www.facebook.com/dungnguyen260103",
                                "story_bucket": {
                                    "nodes": []
                                },
                                "url": "https://www.facebook.com/dungnguyen260103",
                                "profile_picture": {
                                    "uri": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-1/298876278_1659410691095886_2303696312411106776_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeH7fDUpCtS7TxRwxhDcJnk29jHXBV9RV-T2MdcFX1FX5K8hCHHIYkah8v7RHhG3qq7EIOHeqRnR0gHcB6HC_8vO&_nc_ohc=2IK_OjKXf9MAb7Izcti&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfD2q54Xg62U5XQ-PvfffwV_9QDmUoi6ZL_NUl5olWR5tQ&oe=66229E45",
                                    "width": 40,
                                    "height": 40,
                                    "scale": 1
                                },
                                "__isContextualProfile": "User"
                            },
                            "cursor": "AQHRTX4JEB86Dzr4eYnRfPg-E0Rhg-TAdG7k1SO37986GnHwplxFrbSciWeAkR5fRXoZ1Jkvi0U9goTKwL_apd3G-Q"
                        },
                        {
                            "feedback_reaction_info": {
                                "face_image": {
                                    "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An_EjZkxLL70Wj-QVF5bQc6a1UbfBdeaindMayM5EB_nn6ZbIDF4U4rIKO9ISgyJppdBzZM3T20shDptNixRsCGCU8YNtZNKquX5opCN3SYVdwkNT9uoGFDh8UtV4G0.png?ccb=10-5&oh=00_AfDV4r7igtXZ0tBv7FMWxrMmqWEB0sC4g9L6LC7fpdeEHg&oe=664456F5&_nc_sid=7da55a"
                                },
                                "id": "1635855486666999"
                            },
                            "node": {
                                "id": "100003652689319",
                                "__typename": "User",
                                "__isActor": "User",
                                "mutual_friends": {
                                    "count": 0
                                },
                                "__isProfile": "User",
                                "can_viewer_message": true,
                                "friendship_status": "CAN_REQUEST",
                                "subscribe_status": "CANNOT_SUBSCRIBE",
                                "secondary_subscribe_status": "REGULAR_FOLLOW",
                                "invite_status_in_feedback": "NOT_INVITABLE",
                                "follower_invite_status_in_feedback": "NOT_INVITABLE",
                                "name": "Cao Duy Khánh",
                                "__isEntity": "User",
                                "profile_url": "https://www.facebook.com/cao.duykhanh.35",
                                "story_bucket": {
                                    "nodes": []
                                },
                                "url": "https://www.facebook.com/cao.duykhanh.35",
                                "profile_picture": {
                                    "uri": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-1/362948845_3019125821552478_2620523253243371038_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=103&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeF8YgPDge6G7ZBuUDm2mKWOu_iu4rRe7-i7-K7itF7v6BU8W8ilNMNXTD7JfUf-Xen9upEm-hacOtnO9NsJd73S&_nc_ohc=b7kMxpzslDEAb6s2zk3&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfAzC8EKJlEDi44N3wKPBkelGAtAOmT3bGO_xjQl9ZDeNQ&oe=6622CA64",
                                    "width": 40,
                                    "height": 40,
                                    "scale": 1
                                },
                                "__isContextualProfile": "User"
                            },
                            "cursor": "AQHRqbGP3IeAhmFP7sqMPEQZyGND6ZjxlbNm8keNrZXgPTvhQY1I8dFZYEmflp78S-s58Hv0Veooahr9brcZxI1MQQ"
                        },
                        {
                            "feedback_reaction_info": {
                                "face_image": {
                                    "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An_EjZkxLL70Wj-QVF5bQc6a1UbfBdeaindMayM5EB_nn6ZbIDF4U4rIKO9ISgyJppdBzZM3T20shDptNixRsCGCU8YNtZNKquX5opCN3SYVdwkNT9uoGFDh8UtV4G0.png?ccb=10-5&oh=00_AfDV4r7igtXZ0tBv7FMWxrMmqWEB0sC4g9L6LC7fpdeEHg&oe=664456F5&_nc_sid=7da55a"
                                },
                                "id": "1635855486666999"
                            },
                            "node": {
                                "id": "100039312019815",
                                "__typename": "User",
                                "__isActor": "User",
                                "mutual_friends": {
                                    "count": 0
                                },
                                "__isProfile": "User",
                                "can_viewer_message": true,
                                "friendship_status": "CAN_REQUEST",
                                "subscribe_status": "CAN_SUBSCRIBE",
                                "secondary_subscribe_status": "REGULAR_FOLLOW",
                                "invite_status_in_feedback": "NOT_INVITABLE",
                                "follower_invite_status_in_feedback": "NOT_INVITABLE",
                                "name": "Vũ Văn Hải",
                                "__isEntity": "User",
                                "profile_url": "https://www.facebook.com/hait7777",
                                "story_bucket": {
                                    "nodes": []
                                },
                                "url": "https://www.facebook.com/hait7777",
                                "profile_picture": {
                                    "uri": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.30808-1/435700402_1099654068021650_4044320080558019131_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=108&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHXJfxigALO8rWMfmabaKpszcdjqwEMn53Nx2OrAQyfncLPj1TgAnkR1Qcl_rwBAqmJSdZXLEuoIXc-3wKTBuSo&_nc_ohc=zkdWzAkyb3MAb4YeBtl&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfDNu9avO8QJpQPmR2F8qUoyQYNGxx8cQUjVQBcHamL9yA&oe=6622ADD4",
                                    "width": 40,
                                    "height": 40,
                                    "scale": 1
                                },
                                "__isContextualProfile": "User"
                            },
                            "cursor": "AQHRSoTwGa_dS74spSkqLWwskAeuvqMUCV2q7GsEblAXIosDcYRA4qQTybApywUoZAF-AERm5QQ7QAFo3GY3cHQ2Dg"
                        },
                        {
                            "feedback_reaction_info": {
                                "face_image": {
                                    "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An_EjZkxLL70Wj-QVF5bQc6a1UbfBdeaindMayM5EB_nn6ZbIDF4U4rIKO9ISgyJppdBzZM3T20shDptNixRsCGCU8YNtZNKquX5opCN3SYVdwkNT9uoGFDh8UtV4G0.png?ccb=10-5&oh=00_AfDV4r7igtXZ0tBv7FMWxrMmqWEB0sC4g9L6LC7fpdeEHg&oe=664456F5&_nc_sid=7da55a"
                                },
                                "id": "1635855486666999"
                            },
                            "node": {
                                "id": "100004497138480",
                                "__typename": "User",
                                "__isActor": "User",
                                "mutual_friends": {
                                    "count": 0
                                },
                                "__isProfile": "User",
                                "can_viewer_message": true,
                                "friendship_status": "CAN_REQUEST",
                                "subscribe_status": "CANNOT_SUBSCRIBE",
                                "secondary_subscribe_status": "REGULAR_FOLLOW",
                                "invite_status_in_feedback": "NOT_INVITABLE",
                                "follower_invite_status_in_feedback": "NOT_INVITABLE",
                                "name": "Thân Thuấn",
                                "__isEntity": "User",
                                "profile_url": "https://www.facebook.com/thuanbgutc",
                                "story_bucket": {
                                    "nodes": [
                                        {
                                            "should_show_close_friend_badge": false,
                                            "id": "1606633572707087",
                                            "first_story_to_show": null
                                        }
                                    ]
                                },
                                "url": "https://www.facebook.com/thuanbgutc",
                                "profile_picture": {
                                    "uri": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.30808-1/279447273_2063764350450116_2426513451809271643_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=101&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEoAWfc8ClKeGQraBj5MF7BNOoqj9ez4jU06iqP17PiNXpnW2t797rIxzLPKdxnyv_UtV2RSEEaKcKqeAgAuWSU&_nc_ohc=TVDcmetUQAAAb5_qOs-&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfCYagrGcy_uCfPhQe75TMRXt94jNOdhWiUSlHs80LmhGw&oe=6622C6BE",
                                    "width": 40,
                                    "height": 40,
                                    "scale": 1
                                },
                                "__isContextualProfile": "User"
                            },
                            "cursor": "AQHRnPEFvUHBIoPhJY-hob0A0vNsNxwPQIOQ8OXKc5dp4r0RiAU4ykdgWqlH6upPxYNNVJ32SRZhW3-GFueoNYMTIw"
                        },
                        {
                            "feedback_reaction_info": {
                                "face_image": {
                                    "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An_EjZkxLL70Wj-QVF5bQc6a1UbfBdeaindMayM5EB_nn6ZbIDF4U4rIKO9ISgyJppdBzZM3T20shDptNixRsCGCU8YNtZNKquX5opCN3SYVdwkNT9uoGFDh8UtV4G0.png?ccb=10-5&oh=00_AfDV4r7igtXZ0tBv7FMWxrMmqWEB0sC4g9L6LC7fpdeEHg&oe=664456F5&_nc_sid=7da55a"
                                },
                                "id": "1635855486666999"
                            },
                            "node": {
                                "id": "100008336071425",
                                "__typename": "User",
                                "__isActor": "User",
                                "mutual_friends": {
                                    "count": 0
                                },
                                "__isProfile": "User",
                                "can_viewer_message": true,
                                "friendship_status": "CAN_REQUEST",
                                "subscribe_status": "CAN_SUBSCRIBE",
                                "secondary_subscribe_status": "REGULAR_FOLLOW",
                                "invite_status_in_feedback": "NOT_INVITABLE",
                                "follower_invite_status_in_feedback": "NOT_INVITABLE",
                                "name": "Tạ Tuyên",
                                "__isEntity": "User",
                                "profile_url": "https://www.facebook.com/tuyen.mobie",
                                "story_bucket": {
                                    "nodes": [
                                        {
                                            "should_show_close_friend_badge": false,
                                            "id": "2215283658759482",
                                            "first_story_to_show": null
                                        }
                                    ]
                                },
                                "url": "https://www.facebook.com/tuyen.mobie",
                                "profile_picture": {
                                    "uri": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-1/336387851_937453590761265_3917606531992551621_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=106&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHzbXas3fRWEql3uF1zN712t0Gy_QyYTC63QbL9DJhMLmnMnMTUMxy2PnW_flird4eHfWP0XvIRagF4iQdm9L5r&_nc_ohc=H5gi5D6x86gAb6L4ltM&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfBvOEzUwLH1Aj-JcOTwnjSgO8iy5YiJJxt4lpz3U5I3Gw&oe=6622BF49",
                                    "width": 40,
                                    "height": 40,
                                    "scale": 1
                                },
                                "__isContextualProfile": "User"
                            },
                            "cursor": "AQHR6wRHI4z4JKt_t_91jTqdTkEHbdr9Zr_kD-jH6OA8paT6Ud12ni1_V4YXdZnUZETFUmp55ZNAXe8WGB46HQOaJQ"
                        },
                        {
                            "feedback_reaction_info": {
                                "face_image": {
                                    "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An_EjZkxLL70Wj-QVF5bQc6a1UbfBdeaindMayM5EB_nn6ZbIDF4U4rIKO9ISgyJppdBzZM3T20shDptNixRsCGCU8YNtZNKquX5opCN3SYVdwkNT9uoGFDh8UtV4G0.png?ccb=10-5&oh=00_AfDV4r7igtXZ0tBv7FMWxrMmqWEB0sC4g9L6LC7fpdeEHg&oe=664456F5&_nc_sid=7da55a"
                                },
                                "id": "1635855486666999"
                            },
                            "node": {
                                "id": "100027362831481",
                                "__typename": "User",
                                "__isActor": "User",
                                "mutual_friends": {
                                    "count": 0
                                },
                                "__isProfile": "User",
                                "can_viewer_message": true,
                                "friendship_status": "CAN_REQUEST",
                                "subscribe_status": "CAN_SUBSCRIBE",
                                "secondary_subscribe_status": "REGULAR_FOLLOW",
                                "invite_status_in_feedback": "NOT_INVITABLE",
                                "follower_invite_status_in_feedback": "NOT_INVITABLE",
                                "name": "Khang️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️️",
                                "__isEntity": "User",
                                "profile_url": "https://www.facebook.com/0x1x2x0x",
                                "story_bucket": {
                                    "nodes": []
                                },
                                "url": "https://www.facebook.com/0x1x2x0x",
                                "profile_picture": {
                                    "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t1.30497-1/143086968_2856368904622192_1959732218791162458_n.png?stp=cp0_dst-png_p40x40&_nc_cat=1&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEMZKdokFQ2ymhOl1NND_oRso2H55p0AlGyjYfnmnQCURYu-UsDjvYUE-dqA6odpzWcfUDFw6dJQvx_6ZgK9gAB&_nc_ohc=kNSgHQLZ6doAb7eTDui&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfBWiyBh7wX0sb7SAo4Q6iwfJfU1dN8mADNIA5JF0SsvKA&oe=66445C78",
                                    "width": 40,
                                    "height": 40,
                                    "scale": 1
                                },
                                "__isContextualProfile": "User"
                            },
                            "cursor": "AQHRgMvZQbb5RGeIB8yOC2Z-svWmxNPt8-F3TKUQQqYgB6jBJouvoyB_RcrpxHG5nwYA1hKFnhliyU7RlwsJ-FEAvg"
                        },
                        {
                            "feedback_reaction_info": {
                                "face_image": {
                                    "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9p73Z-J6BigKATVmJnv53DNXQAEqX7Bf69Aah4Q8ikh6updQ9sTv44zxvrmYlc_mjFRuqFvI5iVY-ORXiUPh6A4a7j3OJyZXKE1IIBuQVRadZLW-RAJ-TZJVy3KA.png?ccb=10-5&oh=00_AfB1RTUFGpDhle3ev4_shKaMwb-ZYvv3JKsX8cVCcIQpxQ&oe=664438C8&_nc_sid=7da55a"
                                },
                                "id": "115940658764963"
                            },
                            "node": {
                                "id": "100010792512779",
                                "__typename": "User",
                                "__isActor": "User",
                                "mutual_friends": {
                                    "count": 0
                                },
                                "__isProfile": "User",
                                "can_viewer_message": true,
                                "friendship_status": "CAN_REQUEST",
                                "subscribe_status": "CANNOT_SUBSCRIBE",
                                "secondary_subscribe_status": "REGULAR_FOLLOW",
                                "invite_status_in_feedback": "NOT_INVITABLE",
                                "follower_invite_status_in_feedback": "NOT_INVITABLE",
                                "name": "Nguyễn Quốc Hưng",
                                "__isEntity": "User",
                                "profile_url": "https://www.facebook.com/profile.php?id=100010792512779",
                                "story_bucket": {
                                    "nodes": []
                                },
                                "url": "https://www.facebook.com/profile.php?id=100010792512779",
                                "profile_picture": {
                                    "uri": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.30808-1/300384268_1789842971385436_1620731074559822069_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=110&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHUnW3cXZkznxGHh5ZLnKG6VT6p_2ShmIhVPqn_ZKGYiA95T_nwt5yidw51jJH7DPb0Sfo9PPGywiozCsEMFDt5&_nc_ohc=4kW7Hze_BmgAb6YSkZd&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfDAq8jJaXeoNdp-3TD9I9S-lZk1i77xxElGBkv3g_yaNA&oe=6622A285",
                                    "width": 40,
                                    "height": 40,
                                    "scale": 1
                                },
                                "__isContextualProfile": "User"
                            },
                            "cursor": "AQHRElfl0I-qTAhna57UjPOl7IJ1B0v2rvsCQ8jtpp1eFzJXlkkhXPcAR0yH_lXBw6pph3Elwzz3ET9vWs2oJDJu7A"
                        },
                        {
                            "feedback_reaction_info": {
                                "face_image": {
                                    "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An_EjZkxLL70Wj-QVF5bQc6a1UbfBdeaindMayM5EB_nn6ZbIDF4U4rIKO9ISgyJppdBzZM3T20shDptNixRsCGCU8YNtZNKquX5opCN3SYVdwkNT9uoGFDh8UtV4G0.png?ccb=10-5&oh=00_AfDV4r7igtXZ0tBv7FMWxrMmqWEB0sC4g9L6LC7fpdeEHg&oe=664456F5&_nc_sid=7da55a"
                                },
                                "id": "1635855486666999"
                            },
                            "node": {
                                "id": "100024467683242",
                                "__typename": "User",
                                "__isActor": "User",
                                "mutual_friends": {
                                    "count": 0
                                },
                                "__isProfile": "User",
                                "can_viewer_message": false,
                                "friendship_status": "CANNOT_REQUEST",
                                "subscribe_status": "CAN_SUBSCRIBE",
                                "secondary_subscribe_status": "REGULAR_FOLLOW",
                                "invite_status_in_feedback": "NOT_INVITABLE",
                                "follower_invite_status_in_feedback": "NOT_INVITABLE",
                                "name": "Nguyễn Hưng",
                                "__isEntity": "User",
                                "profile_url": "https://www.facebook.com/nguyentuanhung.dev.codetool",
                                "story_bucket": {
                                    "nodes": [
                                        {
                                            "should_show_close_friend_badge": false,
                                            "id": "466632950828957",
                                            "first_story_to_show": null
                                        }
                                    ]
                                },
                                "url": "https://www.facebook.com/nguyentuanhung.dev.codetool",
                                "profile_picture": {
                                    "uri": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-1/344259876_1717007275384750_8037801988402286671_n.jpg?stp=c0.11.40.40a_cp0_dst-jpg_p40x40&_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEtcOKthqZtvCbwZee_2NlcSuKzkomi6VtK4rOSiaLpWywHi21xJ37e3apSyy3bLZ2NnFhuinRysP27KzdRBxBA&_nc_ohc=dkKPq6rYS-4Ab4sIqSs&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfBGQhXUlNeXyI8s_mvkzIHRzGhQBtF-mzfW5-IZqCRzlg&oe=6622BFD6",
                                    "width": 40,
                                    "height": 40,
                                    "scale": 1
                                },
                                "__isContextualProfile": "User"
                            },
                            "cursor": "AQHR6jFac45tjWDNRI7dYi5v3fJx6ACD_kPWc4E6Z-_4uuGkbewMzMsDyzeVejjhDUT18pTXLDaM6hkfO2dlBQ1BaQ"
                        },
                        {
                            "feedback_reaction_info": {
                                "face_image": {
                                    "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9p73Z-J6BigKATVmJnv53DNXQAEqX7Bf69Aah4Q8ikh6updQ9sTv44zxvrmYlc_mjFRuqFvI5iVY-ORXiUPh6A4a7j3OJyZXKE1IIBuQVRadZLW-RAJ-TZJVy3KA.png?ccb=10-5&oh=00_AfB1RTUFGpDhle3ev4_shKaMwb-ZYvv3JKsX8cVCcIQpxQ&oe=664438C8&_nc_sid=7da55a"
                                },
                                "id": "115940658764963"
                            },
                            "node": {
                                "id": "100013447081375",
                                "__typename": "User",
                                "__isActor": "User",
                                "mutual_friends": {
                                    "count": 0
                                },
                                "__isProfile": "User",
                                "can_viewer_message": true,
                                "friendship_status": "CAN_REQUEST",
                                "subscribe_status": "CAN_SUBSCRIBE",
                                "secondary_subscribe_status": "REGULAR_FOLLOW",
                                "invite_status_in_feedback": "NOT_INVITABLE",
                                "follower_invite_status_in_feedback": "NOT_INVITABLE",
                                "name": "Phạm Hà Anh",
                                "__isEntity": "User",
                                "profile_url": "https://www.facebook.com/ph.hah04",
                                "story_bucket": {
                                    "nodes": [
                                        {
                                            "should_show_close_friend_badge": false,
                                            "id": "1267162907075267",
                                            "first_story_to_show": null
                                        }
                                    ]
                                },
                                "url": "https://www.facebook.com/ph.hah04",
                                "profile_picture": {
                                    "uri": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.30808-1/404720747_1890391921419026_749041348802743273_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=101&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEihVuKUyE5kChZV9w1X7gQBoSBzvX3eJ0GhIHO9fd4nWrkvcFH-cjqJwihOqu8HDMgYM3l4nFxhfDdDLk6QvTl&_nc_ohc=UMl8eh6LF0cAb43OU78&_nc_oc=Adj_lPe1LdNS3Vloe73A-_KtXGERKmdq5QJV9ZWY-QA1M-YfeM7W-7VaY7Yo3cf7x5w&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfCVZPK6JMUUbO77c9fmoBDCIBsil6XRdrsJgGw0rkfz1g&oe=6622B5B8",
                                    "width": 40,
                                    "height": 40,
                                    "scale": 1
                                },
                                "__isContextualProfile": "User"
                            },
                            "cursor": "AQHRx3HtkoCfQwYSZGku7lDsgKMQpzunn-UNrWyty2mIF9J789STtKoNxMUSG906GLuA8DOL2cHsjJjlA4UE_9208w"
                        },
                        {
                            "feedback_reaction_info": {
                                "face_image": {
                                    "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An_EjZkxLL70Wj-QVF5bQc6a1UbfBdeaindMayM5EB_nn6ZbIDF4U4rIKO9ISgyJppdBzZM3T20shDptNixRsCGCU8YNtZNKquX5opCN3SYVdwkNT9uoGFDh8UtV4G0.png?ccb=10-5&oh=00_AfDV4r7igtXZ0tBv7FMWxrMmqWEB0sC4g9L6LC7fpdeEHg&oe=664456F5&_nc_sid=7da55a"
                                },
                                "id": "1635855486666999"
                            },
                            "node": {
                                "id": "100004290781203",
                                "__typename": "User",
                                "__isActor": "User",
                                "mutual_friends": {
                                    "count": 0
                                },
                                "__isProfile": "User",
                                "can_viewer_message": true,
                                "friendship_status": "CAN_REQUEST",
                                "subscribe_status": "CAN_SUBSCRIBE",
                                "secondary_subscribe_status": "REGULAR_FOLLOW",
                                "invite_status_in_feedback": "NOT_INVITABLE",
                                "follower_invite_status_in_feedback": "NOT_INVITABLE",
                                "name": "Nguyễn Hiệp",
                                "__isEntity": "User",
                                "profile_url": "https://www.facebook.com/hiepnguyen.nuce",
                                "story_bucket": {
                                    "nodes": [
                                        {
                                            "should_show_close_friend_badge": false,
                                            "id": "1843273572351442",
                                            "first_story_to_show": null
                                        }
                                    ]
                                },
                                "url": "https://www.facebook.com/hiepnguyen.nuce",
                                "profile_picture": {
                                    "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.30808-1/241203026_2006309989522008_6986451210315619478_n.jpg?stp=c0.5.40.40a_cp0_dst-jpg_p40x40&_nc_cat=105&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHijgRUl6Nz8uahBUZVho6aahMKKUsjmatqEwopSyOZqyipJrFq_l2f07ZYKTy1Ln7ZDGBqwsJ7tgr79q70i9gj&_nc_ohc=wajCQsybAO8Ab57cb0R&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfCMWls4F_WclThJAo_rvhnrnL29RNNXzOSSBx0f5-9Yxw&oe=6622C6E2",
                                    "width": 40,
                                    "height": 40,
                                    "scale": 1
                                },
                                "__isContextualProfile": "User"
                            },
                            "cursor": "AQHR285aYAjLqjF82HdkhE9DQBtJ4zmstsLfGXBmqbbTa8kYDjmlm6dcRCqkod9Dr4UgLLyv72y3Jg9XQg9nWxhm7Q"
                        }
                    ],
                    "page_info": {
                        "has_next_page": true,
                        "end_cursor": "AQHRpqHiPg30i_QwFBJUGMyztwRDzAOwd9PhsnREMxszwZnCmEQFrdQEhZzitqNXBMxh_QDw4OQ0Fr8YgJCj-D1Mow"
                    }
                },
                "id": "ZmVlZGJhY2s6NzUyMzM3NzYwNzY4NDQxMw=="
            }
        },
        "extensions": {
            "prefetch_uris_v2": [
                {
                    "uri": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-1/362948845_3019125821552478_2620523253243371038_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=103&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeF8YgPDge6G7ZBuUDm2mKWOu_iu4rRe7-i7-K7itF7v6BU8W8ilNMNXTD7JfUf-Xen9upEm-hacOtnO9NsJd73S&_nc_ohc=b7kMxpzslDEAb6s2zk3&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfAzC8EKJlEDi44N3wKPBkelGAtAOmT3bGO_xjQl9ZDeNQ&oe=6622CA64",
                    "label": null
                },
                {
                    "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t1.30497-1/143086968_2856368904622192_1959732218791162458_n.png?stp=cp0_dst-png_p40x40&_nc_cat=1&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEMZKdokFQ2ymhOl1NND_oRso2H55p0AlGyjYfnmnQCURYu-UsDjvYUE-dqA6odpzWcfUDFw6dJQvx_6ZgK9gAB&_nc_ohc=kNSgHQLZ6doAb7eTDui&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfBWiyBh7wX0sb7SAo4Q6iwfJfU1dN8mADNIA5JF0SsvKA&oe=66445C78",
                    "label": null
                },
                {
                    "uri": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-1/298876278_1659410691095886_2303696312411106776_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeH7fDUpCtS7TxRwxhDcJnk29jHXBV9RV-T2MdcFX1FX5K8hCHHIYkah8v7RHhG3qq7EIOHeqRnR0gHcB6HC_8vO&_nc_ohc=2IK_OjKXf9MAb7Izcti&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfD2q54Xg62U5XQ-PvfffwV_9QDmUoi6ZL_NUl5olWR5tQ&oe=66229E45",
                    "label": null
                },
                {
                    "uri": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-1/336387851_937453590761265_3917606531992551621_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=106&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHzbXas3fRWEql3uF1zN712t0Gy_QyYTC63QbL9DJhMLmnMnMTUMxy2PnW_flird4eHfWP0XvIRagF4iQdm9L5r&_nc_ohc=H5gi5D6x86gAb6L4ltM&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfBvOEzUwLH1Aj-JcOTwnjSgO8iy5YiJJxt4lpz3U5I3Gw&oe=6622BF49",
                    "label": null
                },
                {
                    "uri": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.30808-1/279447273_2063764350450116_2426513451809271643_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=101&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEoAWfc8ClKeGQraBj5MF7BNOoqj9ez4jU06iqP17PiNXpnW2t797rIxzLPKdxnyv_UtV2RSEEaKcKqeAgAuWSU&_nc_ohc=TVDcmetUQAAAb5_qOs-&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfCYagrGcy_uCfPhQe75TMRXt94jNOdhWiUSlHs80LmhGw&oe=6622C6BE",
                    "label": null
                },
                {
                    "uri": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.30808-1/300384268_1789842971385436_1620731074559822069_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=110&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHUnW3cXZkznxGHh5ZLnKG6VT6p_2ShmIhVPqn_ZKGYiA95T_nwt5yidw51jJH7DPb0Sfo9PPGywiozCsEMFDt5&_nc_ohc=4kW7Hze_BmgAb6YSkZd&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfDAq8jJaXeoNdp-3TD9I9S-lZk1i77xxElGBkv3g_yaNA&oe=6622A285",
                    "label": null
                },
                {
                    "uri": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.30808-1/435700402_1099654068021650_4044320080558019131_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=108&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHXJfxigALO8rWMfmabaKpszcdjqwEMn53Nx2OrAQyfncLPj1TgAnkR1Qcl_rwBAqmJSdZXLEuoIXc-3wKTBuSo&_nc_ohc=zkdWzAkyb3MAb4YeBtl&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfDNu9avO8QJpQPmR2F8qUoyQYNGxx8cQUjVQBcHamL9yA&oe=6622ADD4",
                    "label": null
                },
                {
                    "uri": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-1/344259876_1717007275384750_8037801988402286671_n.jpg?stp=c0.11.40.40a_cp0_dst-jpg_p40x40&_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEtcOKthqZtvCbwZee_2NlcSuKzkomi6VtK4rOSiaLpWywHi21xJ37e3apSyy3bLZ2NnFhuinRysP27KzdRBxBA&_nc_ohc=dkKPq6rYS-4Ab4sIqSs&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfBGQhXUlNeXyI8s_mvkzIHRzGhQBtF-mzfW5-IZqCRzlg&oe=6622BFD6",
                    "label": null
                },
                {
                    "uri": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.30808-1/404720747_1890391921419026_749041348802743273_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=101&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEihVuKUyE5kChZV9w1X7gQBoSBzvX3eJ0GhIHO9fd4nWrkvcFH-cjqJwihOqu8HDMgYM3l4nFxhfDdDLk6QvTl&_nc_ohc=UMl8eh6LF0cAb43OU78&_nc_oc=Adj_lPe1LdNS3Vloe73A-_KtXGERKmdq5QJV9ZWY-QA1M-YfeM7W-7VaY7Yo3cf7x5w&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfCVZPK6JMUUbO77c9fmoBDCIBsil6XRdrsJgGw0rkfz1g&oe=6622B5B8",
                    "label": null
                },
                {
                    "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.30808-1/241203026_2006309989522008_6986451210315619478_n.jpg?stp=c0.5.40.40a_cp0_dst-jpg_p40x40&_nc_cat=105&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHijgRUl6Nz8uahBUZVho6aahMKKUsjmatqEwopSyOZqyipJrFq_l2f07ZYKTy1Ln7ZDGBqwsJ7tgr79q70i9gj&_nc_ohc=wajCQsybAO8Ab57cb0R&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfCMWls4F_WclThJAo_rvhnrnL29RNNXzOSSBx0f5-9Yxw&oe=6622C6E2",
                    "label": null
                }
            ],
            "is_final": true
        }
    }
}
```
</details>
