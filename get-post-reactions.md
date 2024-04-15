# APIs-Facebook-no-cookie-token
API lấy data facebook không cần dùng cookie hay token
HOÀN TOÀN MIỄN PHÍ

<details>

<summary>Get reactions (cảm xúc) của bài viết</summary>


```http
GET http://graph.scanfb.top/graphql?action=post_reactions&post_id=&cursor=&access_token=
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `access_token` | `string` | **Bắt buộc**. Miễn phí, liên hệ Kiệt để nhận Token |
| `post_id` | `string` | **Bắt buộc**. ID bài viết, dạng số, không có dấu _ |
| `cursor` | `string` |  Paginate |


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
                                "id": "100056011867845",
                                "__typename": "User",
                                "__isActor": "User",
                                "mutual_friends": {
                                    "count": 0
                                },
                                "__isProfile": "User",
                                "can_viewer_message": true,
                                "friendship_status": "CANNOT_REQUEST",
                                "subscribe_status": "CAN_SUBSCRIBE",
                                "secondary_subscribe_status": "REGULAR_FOLLOW",
                                "invite_status_in_feedback": "NOT_INVITABLE",
                                "follower_invite_status_in_feedback": "NOT_INVITABLE",
                                "name": "Danh Tr",
                                "__isEntity": "User",
                                "profile_url": "https://www.facebook.com/profile.php?id=100056011867845",
                                "story_bucket": {
                                    "nodes": []
                                },
                                "url": "https://www.facebook.com/profile.php?id=100056011867845",
                                "profile_picture": {
                                    "uri": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.30808-1/431876995_886133106597077_3347725015372346796_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=109&ccb=1-7&_nc_sid=5f2048&_nc_ohc=tHBhwOd_kiUAb7_5s9F&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfBvn0WbiRnHiKBjOWpMthR2d_elBuXE9cpDFQ_9lIYyAQ&oe=6622A4DE",
                                    "width": 40,
                                    "height": 40,
                                    "scale": 1
                                },
                                "__isContextualProfile": "User"
                            },
                            "cursor": "AQHRK5xwv-6LfpL1sx_f5OwzSHhidz12oARLARZ7Tq-9RtK51kjFX4oTrAgZa_I88jiXp-h0b4JyYF0xQjT2e4WJIA"
                        },
                        {
                            "feedback_reaction_info": {
                                "face_image": {
                                    "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An_EjZkxLL70Wj-QVF5bQc6a1UbfBdeaindMayM5EB_nn6ZbIDF4U4rIKO9ISgyJppdBzZM3T20shDptNixRsCGCU8YNtZNKquX5opCN3SYVdwkNT9uoGFDh8UtV4G0.png?ccb=10-5&oh=00_AfDV4r7igtXZ0tBv7FMWxrMmqWEB0sC4g9L6LC7fpdeEHg&oe=664456F5&_nc_sid=7da55a"
                                },
                                "id": "1635855486666999"
                            },
                            "node": {
                                "id": "100012869944176",
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
                                "name": "Trần Thiên Hoàng",
                                "__isEntity": "User",
                                "profile_url": "https://www.facebook.com/TranThienHoang1523",
                                "story_bucket": {
                                    "nodes": []
                                },
                                "url": "https://www.facebook.com/TranThienHoang1523",
                                "profile_picture": {
                                    "uri": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-1/431316144_1883877145384599_7502945784751996785_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=103&ccb=1-7&_nc_sid=5f2048&_nc_ohc=1MhMhmNbzM8Ab494fVs&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfC6qfdKKdOw_XzeqXGMIQgKbJQTdgKRSXCZeClB2k8QIQ&oe=6622B867",
                                    "width": 40,
                                    "height": 40,
                                    "scale": 1
                                },
                                "__isContextualProfile": "User"
                            },
                            "cursor": "AQHRq00SxGXL_EPfX4oB3uosgvWWIF9Rd2bji5M5Wno9WzxINgFb79D4u6v-c4HumknW_gKhcoZ33dC9c00v9CfmVg"
                        },
                        {
                            "feedback_reaction_info": {
                                "face_image": {
                                    "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An_EjZkxLL70Wj-QVF5bQc6a1UbfBdeaindMayM5EB_nn6ZbIDF4U4rIKO9ISgyJppdBzZM3T20shDptNixRsCGCU8YNtZNKquX5opCN3SYVdwkNT9uoGFDh8UtV4G0.png?ccb=10-5&oh=00_AfDV4r7igtXZ0tBv7FMWxrMmqWEB0sC4g9L6LC7fpdeEHg&oe=664456F5&_nc_sid=7da55a"
                                },
                                "id": "1635855486666999"
                            },
                            "node": {
                                "id": "100005123198852",
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
                                "name": "Mai Anh",
                                "__isEntity": "User",
                                "profile_url": "https://www.facebook.com/maianh.e9bka",
                                "story_bucket": {
                                    "nodes": [
                                        {
                                            "should_show_close_friend_badge": false,
                                            "id": "628704643920814",
                                            "first_story_to_show": null
                                        }
                                    ]
                                },
                                "url": "https://www.facebook.com/maianh.e9bka",
                                "profile_picture": {
                                    "uri": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-1/249269977_1963354893845265_2498030394448694643_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_ohc=5YggtPvgajcAb5R-946&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfCYekJO5oVFVWUKX6GHTqXXY7ndgqRcmybK2T11K-F32w&oe=6622A95B",
                                    "width": 40,
                                    "height": 40,
                                    "scale": 1
                                },
                                "__isContextualProfile": "User"
                            },
                            "cursor": "AQHRmzRRZS05mg6Ktew2BsT9L9ni_qfWNl3bs39sNAqLNyB6fNg8Z7hjdu_FY5AwIkkTOqdGj9REkp3HuxD1qR1QVw"
                        },
                        {
                            "feedback_reaction_info": {
                                "face_image": {
                                    "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An_EjZkxLL70Wj-QVF5bQc6a1UbfBdeaindMayM5EB_nn6ZbIDF4U4rIKO9ISgyJppdBzZM3T20shDptNixRsCGCU8YNtZNKquX5opCN3SYVdwkNT9uoGFDh8UtV4G0.png?ccb=10-5&oh=00_AfDV4r7igtXZ0tBv7FMWxrMmqWEB0sC4g9L6LC7fpdeEHg&oe=664456F5&_nc_sid=7da55a"
                                },
                                "id": "1635855486666999"
                            },
                            "node": {
                                "id": "100001629622581",
                                "__typename": "User",
                                "__isActor": "User",
                                "mutual_friends": {
                                    "count": 0
                                },
                                "__isProfile": "User",
                                "can_viewer_message": true,
                                "friendship_status": "CANNOT_REQUEST",
                                "subscribe_status": "CANNOT_SUBSCRIBE",
                                "secondary_subscribe_status": "REGULAR_FOLLOW",
                                "invite_status_in_feedback": "NOT_INVITABLE",
                                "follower_invite_status_in_feedback": "NOT_INVITABLE",
                                "name": "Hồ Phan Minh",
                                "__isEntity": "User",
                                "profile_url": "https://www.facebook.com/hophanminh",
                                "story_bucket": {
                                    "nodes": []
                                },
                                "url": "https://www.facebook.com/hophanminh",
                                "profile_picture": {
                                    "uri": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-1/272889344_5162360477161555_6715235937749453079_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=106&ccb=1-7&_nc_sid=5f2048&_nc_ohc=RIWkX80l_1AAb4wQKJh&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfAJygPf2F0nd36yI0ku3OfLb-dProzvbmj5xykQvYX1VA&oe=6622C221",
                                    "width": 40,
                                    "height": 40,
                                    "scale": 1
                                },
                                "__isContextualProfile": "User"
                            },
                            "cursor": "AQHR1eTJ4ccnp3XAQTyPSMUT5skQSnsqOOIOEyFdgPA7MQSZVS_8-keTxoBQ4Pjv9lp8EXZsR2EtFMY9Hx2oi9TEtw"
                        }
                    ],
                    "page_info": {
                        "has_next_page": false,
                        "end_cursor": "AQHRofsYHInGVDW_8X2-1KqgBStRkjemYulmHD-MQGpTcOBsja5fvhsHEw7B8d1RBY50Xp6PUjut3RM2oCDr-tOlnA"
                    }
                },
                "id": "ZmVlZGJhY2s6MjIyMzc0NjYzNDYyNDExMV8yMjIzOTMxMTAxMjcyMzMx"
            }
        },
        "extensions": {
            "prefetch_uris_v2": [
                {
                    "uri": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.30808-1/431876995_886133106597077_3347725015372346796_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=109&ccb=1-7&_nc_sid=5f2048&_nc_ohc=tHBhwOd_kiUAb7_5s9F&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfBvn0WbiRnHiKBjOWpMthR2d_elBuXE9cpDFQ_9lIYyAQ&oe=6622A4DE",
                    "label": null
                },
                {
                    "uri": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-1/249269977_1963354893845265_2498030394448694643_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_ohc=5YggtPvgajcAb5R-946&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfCYekJO5oVFVWUKX6GHTqXXY7ndgqRcmybK2T11K-F32w&oe=6622A95B",
                    "label": null
                },
                {
                    "uri": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-1/431316144_1883877145384599_7502945784751996785_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=103&ccb=1-7&_nc_sid=5f2048&_nc_ohc=1MhMhmNbzM8Ab494fVs&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfC6qfdKKdOw_XzeqXGMIQgKbJQTdgKRSXCZeClB2k8QIQ&oe=6622B867",
                    "label": null
                },
                {
                    "uri": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-1/272889344_5162360477161555_6715235937749453079_n.jpg?stp=cp0_dst-jpg_p40x40&_nc_cat=106&ccb=1-7&_nc_sid=5f2048&_nc_ohc=RIWkX80l_1AAb4wQKJh&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfAJygPf2F0nd36yI0ku3OfLb-dProzvbmj5xykQvYX1VA&oe=6622C221",
                    "label": null
                }
            ],
            "is_final": true
        }
    }
}
```
</details>
