# APIs-Facebook-no-cookie-token
API lấy data facebook không cần dùng cookie hay token
HOÀN TOÀN MIỄN PHÍ

<details>

<summary>Tìm kiếm quảng cáo trong Ads Library</summary>


```http
GET http://graph.scanfb.top/search-ads?keyword=laptop&forward_cursor=&collection_token=&access_token=N8o3eySfREuw1pbt3fmcLg
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `keyword` | `string` | **Bắt buộc**. Từ khoá tìm kiếm quảng cáo  |
| `forward_cursor` | `string` | Paginate  |
| `collection_token` | `string` | Paginate  |
| `access_token` | `string` | **Bắt buộc**. Token trên được chia sẽ công khai, nhiều người dùng, request có thể sẽ chậm. Liên hệ Kiệt để nhận Token riêng miễn phí |


### Response

```json
{
    "success": true,
    "message": "",
    "data": {
        "__ar": 1,
        "payload": {
            "isResultComplete": false,
            "results": [
                [
                    {
                        "adid": "0",
                        "adArchiveID": "952254996289312",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 2,
                        "collationID": 1700856193775809,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "248734494998159",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Laptop nhập khẩu Bảo Duy ",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120209895045290002",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": "🔥Xã kho 2.9tr #laptop xách tay Nhật",
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Mua laptop x260 giá 3tr\"},{\"title\":\"X1 Carbon cao cấp giá 5 đến 7 triệu\"},{\"title\":\"Mua balo Bảo Duy 110k hoặc phụ kiện\"},{\"title\":\"Cần tư gặp chuyên gia tư vấn chọn laptop\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Bạn đang quan tâm X270?\",\"is_eligible_for_customized_greeting\":false}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Bạn đang quan tâm X270?\",\"is_eligible_for_customized_greeting\":false}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Bạn đang quan tâm X270?\",\"is_eligible_for_customized_greeting\":false}},\"user_edit\":true,\"surface\":\"visual_editor_new\",\"ai_generated_welcome_message_impression\":false,\"has_ai_generated_welcome_message\":false,\"welcome_message_edited\":true,\"ice_breakers_edited\":true,\"template_id\":\"7735198859833039\"}",
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t42.1790-2/10000000_952255032955975_6315718267493465505_n.?_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFce2g8yXIY8XcxcbFco-U1MFOk6BTcBYEwU6ToFNwFgbwFXKMuuTIilhEpxAe-yFFy5x5QaOuIOY4GbdeXW5S5&_nc_ohc=3VKJGdYZvQEAb5W6VP1&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfBnRCgLiwBM7yxnUaf087mycxTyafnsVFtPrygd2zHakQ&oe=6622B23F",
                                    "video_sd_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t42.1790-2/10000000_942402060799528_9034703092795025214_n.mp4?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFDBuJUDY9zG61jki3RwLdq5eAL98-BXoDl4Av3z4FegMg9BnNSEIEDVf96iYwDKNzRpin9ElUkWLrXPcbzwOwV&_nc_ohc=v530F1Y20KgAb4p7yr-&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfBs_FVeH0uKNngR1qAvUp-OOUFILLHjiVVP0IMCvrk7rg&oe=6622B483",
                                    "watermarked_video_sd_url": "",
                                    "watermarked_video_hd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/436382781_444245668039808_5942615333351326985_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeH7eIB3ucRHVjZKi3_RyPMQKSpCKio1cJopKkIqKjVwmjAtHk4oh_kRs6fMiTyCyswTJMMIw_fArm30BokyTQFG&_nc_ohc=sPwYpuadV_8Ab5XB9f1&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfBCy_EbUzWWTR57xq0CpdjwOupyYwEqm_UpA_qT256V5Q&oe=6622D58F"
                                }
                            ],
                            "creation_time": 1712384657,
                            "page_id": 248734494998159,
                            "page_name": "Laptop nhập khẩu Bảo Duy ",
                            "page_profile_picture_url": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.35426-6/435925049_3545257735724001_2110215452738087076_n.jpg?stp=dst-jpg_s60x60&_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGwF4nFGUvG0iamPiV48PLEyE-llMP1TeHIT6WUw_VN4dPdt9a3FuN5js_K3mZ7T9zh2Y3mDwoCZfjBOXVMmAT9&_nc_ohc=Bew2HpJHMdoAb7vOEuP&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfBn7Nuknqw5ZCZuxpKw9mY8BLkqWzF9ssXuEHYA98clAA&oe=6622A847",
                            "page_categories": {
                                "109527622457518": "Shopping Mall"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Laptop nhập khẩu Bảo Duy",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/436237360_778835084198536_528494299493142311_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHZV8G6rRFrDit7_UbY4-Wlv1U5a4iMHwi_VTlriIwfCPSCeXzYzZiTq_i2hMvANvWMkqGHKXysd9FHTKtIQ7je&_nc_ohc=hi87JlfqriwAb6A_qLZ&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfBWXKMZXNonzt2CO28A0KiyuEQRLYa_rgiBcHNoqPQ0vg&oe=6622C1CF",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "🔥Xã kho 2.9tr #laptop xách tay Nhật<br /> 🔥Ship COD, được kiểm tra, dùng thử<br /> 👉Máy 99% rất mới, pin trâu 4h liên tục<br /> 👉Làm việc văn phòng thì quá dư thừa.<br /> 👉Chơi tốt các game: FIFA Online, Liên Minh, Pubg, MU Online, Minecraft…<br /> ==============<br /> ✅Thinkpad X260 - i5 6300<br /> 👉Op 1: RAM 4G - SSD 128 =&gt; 2.9tr<br /> 👉Op 2: RAM 8G - SSD 256 =&gt; 3.4tr<br /> <br /> ✅Thinkpad X270 - i5 6300<br /> 👉Op 1: RAM 4G - SSD 128 =&gt; 3.1tr<br /> 👉Op 2: RAM 8G - SSD 256 =&gt; 3.5tr<br /> <br /> ✅Thinkpad A285 AMD Ryzen™ 5200<br /> 👉Op 1: RAM 8G - SSD 128 =&gt; 3.9tr<br /> 👉Op 2: RAM 8G - SSD 256 =&gt; 4.4tr<br /> <br /> ✅Thinkpad Thinkpad T470s i5-7300<br /> 👉Op 1: RAM 16G - SSD 128=&gt; 4.9tr<br /> 👉Op 2: RAM 16G - SSD 256 =&gt; 5.5tr<br /> <br /> ✅Thinkpad X1 gen5 - i5 7300<br /> 👉Op 1: RAM 4G - SSD 128 =&gt; 4.9tr<br /> 👉Op 2: RAM 8G - SSD 256 =&gt; 5.5tr<br /> <br /> ✅Thinkpad X1 gen6 - i5 8250<br /> 👉Op 1: RAM 4G - SSD 128 =&gt; 5.5tr<br /> 👉Op 2: RAM 8G - SSD 128 =&gt; 5.9tr<br /> 👉Op 3: RAM 8G - SSD 256 =&gt; 6.5tr<br /> <br /> ✅Thinkpad X1 gen7 - i5 8350<br /> 👉Op 1: RAM 8G - SSD 128 =&gt; 6.9tr<br /> 👉Op 2: RAM 8G - SSD 256 =&gt; 7.5tr<br /> ==============<br /> ✅Mọi người lưu ý, laptop nó có rất nhiều loại, hàng chính hãng, hàng rin, hàng đẹp.... Bên mình là công ty lớn, bán hàng đặt uy tín lên hàng đầu không phải cá nhân nhỏ lẻ bán hàng theo cách vui thì bán, giá cả không niêm yết rõ ràng.<br /> <br /> 🎯Hotline 0935.456.456 ship COD toàn quốc<br /> <br /> 🎯Cửa hàng Hồ Chí Minh: 0978.800.841<br /> 20/5 Tổ 7 Khu Phố 8 - Đường Huỳnh Thị Hai Phường Tân Chánh Hiệp, Quận 12<br /> <br /> 🎯Cửa hàng Đà Nẵng: 0901.004.222<br /> 161 Nguyễn Quang Lâm, Hoà Xuân, Cẩm Lệ<br /> <br /> 🎯Cửa hàng Quảng Trị: 0988.605.555<br /> 42 Nguyễn Du - Hồ Xá - Vĩnh Linh<br /> <br /> 🎯Cửa hàng Hà Nội: 0984.725.638<br /> 5A3 ngõ 673 đường Cổ Điển - X. Tứ Hiệp - H. Thanh Trì"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Laptop nhập khẩu Bảo Duy ",
                            "disclaimer_label": null,
                            "page_like_count": 211,
                            "page_profile_uri": "https://facebook.com/61557704956761",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712300400,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    },
                    {
                        "adid": "0",
                        "adArchiveID": "385597777723048",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": null,
                        "collationID": 1700856193775809,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "248734494998159",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Laptop nhập khẩu Bảo Duy ",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120209895045260002",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": "🔥Xã kho 2.9tr #laptop xách tay Nhật",
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Mua laptop x260 giá 3tr\"},{\"title\":\"X1 Carbon cao cấp giá 5 đến 7 triệu\"},{\"title\":\"Mua balo Bảo Duy 110k hoặc phụ kiện\"},{\"title\":\"Cần tư gặp chuyên gia tư vấn chọn laptop\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Bạn đang quan tâm X270?\",\"is_eligible_for_customized_greeting\":false}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Bạn đang quan tâm X270?\",\"is_eligible_for_customized_greeting\":false}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Bạn đang quan tâm X270?\",\"is_eligible_for_customized_greeting\":false}},\"user_edit\":true,\"surface\":\"visual_editor_new\",\"ai_generated_welcome_message_impression\":false,\"has_ai_generated_welcome_message\":false,\"welcome_message_edited\":true,\"ice_breakers_edited\":true,\"template_id\":\"7735198859833039\"}",
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "https://scontent.fsgn2-5.fna.fbcdn.net/v/t42.1790-2/10000000_385597817723044_718627501883396278_n.?_nc_cat=104&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFG5TZKAlkOQHJcaj5sJHmOp8AObbxBBSqnwA5tvEEFKt5JWVyteRalaq5drdYK7RPeouRH2jYyNm_uKY2q7CpG&_nc_ohc=pbLxPj2NeicAb52elO7&_nc_ht=scontent.fsgn2-5.fna&oh=00_AfArnTA6-0UQsVFCHpQLWRhil9OZ53eOKfJse2k5BtnbqA&oe=6622D70C",
                                    "video_sd_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t42.1790-2/10000000_942402060799528_9034703092795025214_n.mp4?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFDBuJUDY9zG61jki3RwLdq5eAL98-BXoDl4Av3z4FegMg9BnNSEIEDVf96iYwDKNzRpin9ElUkWLrXPcbzwOwV&_nc_ohc=v530F1Y20KgAb4p7yr-&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfBs_FVeH0uKNngR1qAvUp-OOUFILLHjiVVP0IMCvrk7rg&oe=6622B483",
                                    "watermarked_video_sd_url": "",
                                    "watermarked_video_hd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/436162381_400236465977368_1382084989335899124_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEHfussOaA76XL6KKKqftP2becavgy3Zqtt5xq-DLdmq7A_ZYIuNwPXoJDYKL6tJqfraET_PWpd99eLt0GDpVRC&_nc_ohc=FsJwWsn_bUkAb5c99Gg&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfCj03Kz2qE13Wr0ywckVsyWr3qJKk2sJ9Q3fuGU2yeAyA&oe=6622D879"
                                }
                            ],
                            "creation_time": 1712384656,
                            "page_id": 248734494998159,
                            "page_name": "Laptop nhập khẩu Bảo Duy ",
                            "page_profile_picture_url": "https://scontent.fsgn2-5.fna.fbcdn.net/v/t39.35426-6/436108198_430574126147953_4417689710848956806_n.jpg?stp=dst-jpg_s60x60&_nc_cat=104&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFSlbefdIXs2D1vyL55JUlNZZ_fsz6WmEhln9-zPpaYSI9owhzphI6BnAa4WT_zFJYw1y-lEUo2unkyakdZ8mlq&_nc_ohc=QBkiLrC9VEYAb7Xy2EI&_nc_ht=scontent.fsgn2-5.fna&oh=00_AfDQ4NwVFMXpF60Z-yJ_Yg1MXXkgJMYTldLOk9Glwvh84w&oe=6622A69E",
                            "page_categories": {
                                "109527622457518": "Shopping Mall"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Laptop nhập khẩu Bảo Duy",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/436278803_957576495926960_7619296020396954677_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHOKKjkqM30QTCTIfqjDbtW703wdwu03rPvTfB3C7Tes2ZsIl11l_yShB-kulBgx22u-WWAzLXhtibVABYX98AE&_nc_ohc=sjVGh3CufXAAb6ExWjo&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfBd0KlJFvS7LUk4C7_T3ujnNtMdSfjilPFkVoGO8F_b6Q&oe=6622B812",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "🔥Xã kho 2.9tr #laptop xách tay Nhật<br /> 🔥Ship COD, được kiểm tra, dùng thử<br /> 👉Máy 99% rất mới, pin trâu 4h liên tục<br /> 👉Làm việc văn phòng thì quá dư thừa.<br /> 👉Chơi tốt các game: FIFA Online, Liên Minh, Pubg, MU Online, Minecraft…<br /> ==============<br /> ✅Thinkpad X260 - i5 6300<br /> 👉Op 1: RAM 4G - SSD 128 =&gt; 2.9tr<br /> 👉Op 2: RAM 8G - SSD 256 =&gt; 3.4tr<br /> <br /> ✅Thinkpad X270 - i5 6300<br /> 👉Op 1: RAM 4G - SSD 128 =&gt; 3.1tr<br /> 👉Op 2: RAM 8G - SSD 256 =&gt; 3.5tr<br /> <br /> ✅Thinkpad A285 AMD Ryzen™ 5200<br /> 👉Op 1: RAM 8G - SSD 128 =&gt; 3.9tr<br /> 👉Op 2: RAM 8G - SSD 256 =&gt; 4.4tr<br /> <br /> ✅Thinkpad Thinkpad T470s i5-7300<br /> 👉Op 1: RAM 16G - SSD 128=&gt; 4.9tr<br /> 👉Op 2: RAM 16G - SSD 256 =&gt; 5.5tr<br /> <br /> ✅Thinkpad X1 gen5 - i5 7300<br /> 👉Op 1: RAM 4G - SSD 128 =&gt; 4.9tr<br /> 👉Op 2: RAM 8G - SSD 256 =&gt; 5.5tr<br /> <br /> ✅Thinkpad X1 gen6 - i5 8250<br /> 👉Op 1: RAM 4G - SSD 128 =&gt; 5.5tr<br /> 👉Op 2: RAM 8G - SSD 128 =&gt; 5.9tr<br /> 👉Op 3: RAM 8G - SSD 256 =&gt; 6.5tr<br /> <br /> ✅Thinkpad X1 gen7 - i5 8350<br /> 👉Op 1: RAM 8G - SSD 128 =&gt; 6.9tr<br /> 👉Op 2: RAM 8G - SSD 256 =&gt; 7.5tr<br /> ==============<br /> ✅Mọi người lưu ý, laptop nó có rất nhiều loại, hàng chính hãng, hàng rin, hàng đẹp.... Bên mình là công ty lớn, bán hàng đặt uy tín lên hàng đầu không phải cá nhân nhỏ lẻ bán hàng theo cách vui thì bán, giá cả không niêm yết rõ ràng.<br /> <br /> 🎯Hotline 0935.456.456 ship COD toàn quốc<br /> <br /> 🎯Cửa hàng Hồ Chí Minh: 0978.800.841<br /> 20/5 Tổ 7 Khu Phố 8 - Đường Huỳnh Thị Hai Phường Tân Chánh Hiệp, Quận 12<br /> <br /> 🎯Cửa hàng Đà Nẵng: 0901.004.222<br /> 161 Nguyễn Quang Lâm, Hoà Xuân, Cẩm Lệ<br /> <br /> 🎯Cửa hàng Quảng Trị: 0988.605.555<br /> 42 Nguyễn Du - Hồ Xá - Vĩnh Linh<br /> <br /> 🎯Cửa hàng Hà Nội: 0984.725.638<br /> 5A3 ngõ 673 đường Cổ Điển - X. Tứ Hiệp - H. Thanh Trì"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Laptop nhập khẩu Bảo Duy ",
                            "disclaimer_label": null,
                            "page_like_count": 211,
                            "page_profile_uri": "https://facebook.com/61557704956761",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712300400,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "429611012810252",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 2,
                        "collationID": 1386882612215516,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "109431578069085",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Laptop Ipad nhập khẩu Bảo Duy",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120209849871070002",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": "🔥Xã kho 2.9tr #laptop xách tay Nhật",
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Tham khảo laptop x260, 270\"},{\"title\":\"Tham khảo laptop x1 gen5, gen6\"},{\"title\":\"Mua túi xách Bảo Duy 110k\"},{\"title\":\"Mua chuột logitech không dây M220 giá 90k\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Bạn cần tư vấn laptop phải không ạ?\"}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Bạn cần tư vấn laptop phải không ạ?\"}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Bạn cần tư vấn laptop phải không ạ?\"}},\"user_edit\":true,\"surface\":\"visual_editor_new\",\"welcome_message_edited\":true,\"ice_breakers_edited\":true,\"template_id\":\"776001327296703\"}",
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "https://scontent.fsgn2-5.fna.fbcdn.net/v/t42.1790-2/10000000_429611066143580_3698075105397748097_n.?_nc_cat=104&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGj13sW085qxp5AVCAKnnv6DOYyVbvYqZ4M5jJVu9ipnpnS0fDjW2f-IzuuD9E_1zsl4bhfTIM5Ow4ikn326PBd&_nc_ohc=j6igWQcZ0HkAb71AtVd&_nc_ht=scontent.fsgn2-5.fna&oh=00_AfBmB-m7n0QUHhiTQ0jvrXKcmDkMag9EX3EpbFm3l8qeRA&oe=6622A92E",
                                    "video_sd_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t42.1790-2/10000000_1485272248694591_5967674570918226491_n.mp4?_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFwDDcMkdV53PpFJO3Z7yqUg_7UGTY1qPyD_tQZNjWo_PTCPXV2clbQoBs2lu75u56isaAq1eOsvrHbvs8RSavc&_nc_ohc=DckPyzkvq8wAb5O1P9q&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDZ18AAwZTutOlJ3NAtPF7a3NiKvB10ldtRKSrh8P795g&oe=6622AA59",
                                    "watermarked_video_sd_url": "",
                                    "watermarked_video_hd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/435922818_7617147995015691_34155210189981610_n.jpg?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHHn381dA-pEzzxrejjX3dv_43hTjq-bqH_jeFOOr5uoffx0EFa4SRbFfR4MFEzL4MmOoau6cxP3PIw8MUiFoLO&_nc_ohc=o_XjXK-p3MMAb4HMKd3&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfD_txGgH5-WeeuDBJWxwMFrk0rsbV1VjqpodvsxIsoE3w&oe=6622AB9F",
                                    "video_caption_urls": {
                                        "vi_VN": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.2093-6/430909845_291563093953136_5133444519296928769_n.srt?_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHa2Vf_2FmIT-q4Oc6OYohq8_Fli5MDh_vz8WWLkwOH-4sAU-LgzQ7aIVKFF59pGpjtZNuqoS5PUw6UTABAHENN&_nc_ohc=InL070S6TZ8Ab7zondy&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfA-K0E1ygqm2MHbQ1qqQltNOs_Ul9I1YiPVTHWfP3-SqQ&oe=6622C708"
                                    }
                                }
                            ],
                            "creation_time": 1712308917,
                            "page_id": 109431578069085,
                            "page_name": "Laptop Ipad nhập khẩu Bảo Duy",
                            "page_profile_picture_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/435899374_1126487712002344_1477553040344518028_n.jpg?stp=dst-jpg_s60x60&_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeF6JZhilxdXH5_UNVeNO5BqHASW6M5BRLEcBJbozkFEsakqbI4J1Mr_MOgL0ralJki8LjCWW7OJOpXbmC5iU6vz&_nc_ohc=ehTIv4x6tW4Ab5i416N&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfBObApq_gR6yh9T1oyLAqKJdfomYSabvv15JNH7PoCgcA&oe=6622BFE7",
                            "page_categories": {
                                "200600219953504": "Shopping"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Laptop Ipad nhập khẩu Bảo Duy",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/435925036_955216799157958_8687157152971814991_n.jpg?_nc_cat=103&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGaUKlTW066f9Fb6vPK4Izg9m206JPijx72bbTok-KPHmAk3xF8IWEp4rU0xU432YKSHB0PQGMonKOYBgjk2tOE&_nc_ohc=vtLI2c9OmJEAb7gMzSM&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfAyfkgRg_NgDjZajcFDi89KO4nRl5DBzsQ0asRCkXFCzw&oe=6622D8BA",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "🔥Xã kho 2.9tr #laptop xách tay Nhật<br /> 🔥Ship COD, được kiểm tra, dùng thử<br /> 👉Máy 99% rất mới, pin trâu 5h liên tục<br /> 👉Làm việc văn phòng thì quá dư thừa.<br /> 👉Chơi tốt các game: FIFA Online, Liên Minh, Pubg, MU Online, Minecraft…<br /> ==============<br /> ✅Thinkpad X260 - i5 6300<br /> 👉Op 1: RAM 4G - SSD 128 =&gt; 2.9tr<br /> 👉Op 3: RAM 8G - SSD 256 =&gt; 3.3tr<br /> <br /> ✅Thinkpad X270 - i5 6300<br /> 👉Op 1: RAM 4G - SSD 128 =&gt; 3.1tr<br /> 👉Op 3: RAM 8G - SSD 256 =&gt; 3.5tr<br /> <br /> ✅Thinkpad X1 gen5 - i5 7300<br /> 👉Op 1: RAM 4G - SSD 128 =&gt; 4.9tr<br /> 👉Op 2: RAM 8G - SSD 256 =&gt; 5.5tr<br /> <br /> ✅Thinkpad X1 gen6 - i5 8250<br /> 👉Op 1: RAM 4G - SSD 128 =&gt; 5.5tr<br /> 👉Op 2: RAM 8G - SSD 128 =&gt; 5.9tr<br /> ==============<br /> ✅Mọi người lưu ý, laptop nó có rất nhiều loại, hàng chính hãng, hàng rin, hàng đẹp.... Bên mình là công ty lớn, bán hàng đặt uy tín lên hàng đầu không phải cá nhân nhỏ lẻ bán hàng theo cách vui thì bán, giá cả không niêm yết rõ ràng.<br /> <br /> 🎯Hotline 0935.456.456 ship COD toàn quốc<br /> <br /> 🎯Cửa hàng Hồ Chí Minh: 0978.800.841<br /> 20/5 Tổ 7 Khu Phố 8 - Đường Huỳnh Thị Hai Phường Tân Chánh Hiệp, Quận 12<br /> <br /> 🎯Cửa hàng Đà Nẵng: 0901.004.222<br /> 135 Phạm Hùng, Hoà Xuân, Cẩm Lệ<br /> <br /> 🎯Cửa hàng Quảng Trị: 0988.605.555<br /> 42 Nguyễn Du - Hồ Xá - Vĩnh Linh<br /> <br /> 🎯Cửa hàng Hà Nội: 0984.725.638<br /> 5A3 ngõ 673 đường Cổ Điển - X. Tứ Hiệp - H. Thanh Trì"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Laptop Ipad nhập khẩu Bảo Duy",
                            "disclaimer_label": null,
                            "page_like_count": 4167,
                            "page_profile_uri": "https://facebook.com/baoduystore.pc",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712300400,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    },
                    {
                        "adid": "0",
                        "adArchiveID": "981076086918798",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": null,
                        "collationID": 1386882612215516,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "109431578069085",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Laptop Ipad nhập khẩu Bảo Duy",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120209849871040002",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": "🔥Xã kho 2.9tr #laptop xách tay Nhật",
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Tham khảo laptop x260, 270\"},{\"title\":\"Tham khảo laptop x1 gen5, gen6\"},{\"title\":\"Mua túi xách Bảo Duy 110k\"},{\"title\":\"Mua chuột logitech không dây M220 giá 90k\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Bạn cần tư vấn laptop phải không ạ?\"}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Bạn cần tư vấn laptop phải không ạ?\"}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Bạn cần tư vấn laptop phải không ạ?\"}},\"user_edit\":true,\"surface\":\"visual_editor_new\",\"welcome_message_edited\":true,\"ice_breakers_edited\":true,\"template_id\":\"776001327296703\"}",
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t42.1790-2/10000000_981076143585459_4669042735271929290_n.?_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHXXOcTlqHYwp3hNvmkgJQWLuIQbLlKxdwu4hBsuUrF3GxAbn8N8474HR0LGYIJVPHKZlJyH-pnyp--6IllqWo5&_nc_ohc=wQcgFJJVUx0Ab7Br6KN&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfBmL8lddV-0-U7Tmj26IPAUTN5q3aX4onGJaQTyJx3gqA&oe=6622BD5A",
                                    "video_sd_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t42.1790-2/10000000_1485272248694591_5967674570918226491_n.mp4?_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFwDDcMkdV53PpFJO3Z7yqUg_7UGTY1qPyD_tQZNjWo_PTCPXV2clbQoBs2lu75u56isaAq1eOsvrHbvs8RSavc&_nc_ohc=DckPyzkvq8wAb5O1P9q&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDZ18AAwZTutOlJ3NAtPF7a3NiKvB10ldtRKSrh8P795g&oe=6622AA59",
                                    "watermarked_video_sd_url": "",
                                    "watermarked_video_hd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/436118429_274770685683676_528106225369736893_n.jpg?_nc_cat=100&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHJ19l7tt8Uk7ZGGSBXFSsYDG-si8i7D60Mb6yLyLsPrbkEAGbNIVS7ckt3NQCi5HIEBh-DioY1uOI6rERcflDY&_nc_ohc=-XLhH4GpXRcAb7xcP9T&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfBXi5kPUxQzoVssO6vD_DuDdm5sAb-qdlF8g4NUJORGwg&oe=6622AAE9",
                                    "video_caption_urls": {
                                        "vi_VN": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.2093-6/430909845_291563093953136_5133444519296928769_n.srt?_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHa2Vf_2FmIT-q4Oc6OYohq8_Fli5MDh_vz8WWLkwOH-4sAU-LgzQ7aIVKFF59pGpjtZNuqoS5PUw6UTABAHENN&_nc_ohc=InL070S6TZ8Ab7zondy&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfA-K0E1ygqm2MHbQ1qqQltNOs_Ul9I1YiPVTHWfP3-SqQ&oe=6622C708"
                                    }
                                }
                            ],
                            "creation_time": 1712308915,
                            "page_id": 109431578069085,
                            "page_name": "Laptop Ipad nhập khẩu Bảo Duy",
                            "page_profile_picture_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/435977592_735627525068612_7090123070910745643_n.jpg?stp=dst-jpg_s60x60&_nc_cat=106&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeErkXSe9P9c2TnVclpa8QIZi6me5PGoYEGLqZ7k8ahgQYdffZuHr4aEWBdpFXCH3tjLRqd0qk6FHZSt2cL0r9RV&_nc_ohc=NtNJcT1RV70Ab5qK3Pf&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfC1atz8xTUs5J81_WS47QJnyI18cUX24Pb6-PRF5OUMXw&oe=6622ABDC",
                            "page_categories": {
                                "200600219953504": "Shopping"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Laptop Ipad nhập khẩu Bảo Duy",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/436097712_1612463509528566_6922609364375022084_n.jpg?_nc_cat=100&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFnemubSA2Wh1mJPUMwaRODx_AplDHqan7H8CmUMepqfjMIN96JYdgtnJvnhngYeOueUiQiYhkV7OOnMLALdFPL&_nc_ohc=k4vvZDwLGNsAb7FoRRA&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfDk8wqxjAYbF4VFl-q2hSOurskdfuMMilaFEK4Uvzd-CQ&oe=6622A7D5",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "🔥Xã kho 2.9tr #laptop xách tay Nhật<br /> 🔥Ship COD, được kiểm tra, dùng thử<br /> 👉Máy 99% rất mới, pin trâu 5h liên tục<br /> 👉Làm việc văn phòng thì quá dư thừa.<br /> 👉Chơi tốt các game: FIFA Online, Liên Minh, Pubg, MU Online, Minecraft…<br /> ==============<br /> ✅Thinkpad X260 - i5 6300<br /> 👉Op 1: RAM 4G - SSD 128 =&gt; 2.9tr<br /> 👉Op 3: RAM 8G - SSD 256 =&gt; 3.3tr<br /> <br /> ✅Thinkpad X270 - i5 6300<br /> 👉Op 1: RAM 4G - SSD 128 =&gt; 3.1tr<br /> 👉Op 3: RAM 8G - SSD 256 =&gt; 3.5tr<br /> <br /> ✅Thinkpad X1 gen5 - i5 7300<br /> 👉Op 1: RAM 4G - SSD 128 =&gt; 4.9tr<br /> 👉Op 2: RAM 8G - SSD 256 =&gt; 5.5tr<br /> <br /> ✅Thinkpad X1 gen6 - i5 8250<br /> 👉Op 1: RAM 4G - SSD 128 =&gt; 5.5tr<br /> 👉Op 2: RAM 8G - SSD 128 =&gt; 5.9tr<br /> ==============<br /> ✅Mọi người lưu ý, laptop nó có rất nhiều loại, hàng chính hãng, hàng rin, hàng đẹp.... Bên mình là công ty lớn, bán hàng đặt uy tín lên hàng đầu không phải cá nhân nhỏ lẻ bán hàng theo cách vui thì bán, giá cả không niêm yết rõ ràng.<br /> <br /> 🎯Hotline 0935.456.456 ship COD toàn quốc<br /> <br /> 🎯Cửa hàng Hồ Chí Minh: 0978.800.841<br /> 20/5 Tổ 7 Khu Phố 8 - Đường Huỳnh Thị Hai Phường Tân Chánh Hiệp, Quận 12<br /> <br /> 🎯Cửa hàng Đà Nẵng: 0901.004.222<br /> 135 Phạm Hùng, Hoà Xuân, Cẩm Lệ<br /> <br /> 🎯Cửa hàng Quảng Trị: 0988.605.555<br /> 42 Nguyễn Du - Hồ Xá - Vĩnh Linh<br /> <br /> 🎯Cửa hàng Hà Nội: 0984.725.638<br /> 5A3 ngõ 673 đường Cổ Điển - X. Tứ Hiệp - H. Thanh Trì"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Laptop Ipad nhập khẩu Bảo Duy",
                            "disclaimer_label": null,
                            "page_like_count": 4167,
                            "page_profile_uri": "https://facebook.com/baoduystore.pc",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712300400,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "1155330158808000",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 922092299922165,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "107189848084236",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Trung Tâm Laptop Hải Phòng",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120207622598220345",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": null,
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Vị trí của bạn ở đâu?\"},{\"title\":\"Bạn có thể kiểm tra giá sản phẩm được không?\"},{\"title\":\"Tôi có thể mua hàng không?\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting_text\":false}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting_text\":false}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting_text\":false}},\"user_edit\":false,\"surface\":\"visual_editor_new\"}",
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t42.1790-2/10000000_220228744485228_7214894445745018324_n.?_nc_cat=110&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEmaznfrTYevGyz3U1mZAOxj4swLiOZeqePizAuI5l6pxzriIyP0VUNgZPmIt5CRdeSeB2qP8J2OubhVqxfNoNN&_nc_ohc=6khYna_V8WcAb6abBll&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfBxR1p46Qo_Vv1NuhfmohnsQOtfzbrERFXsRt18cJDhxw&oe=6622CFBE",
                                    "video_sd_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t42.1790-2/434385267_1479525602664664_291276645377829770_n.mp4?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEbdsMQD3P6BVXqGarxL4Rj4C4BSloPUpLgLgFKWg9Sknbrq2cuEcJ9sz_x5XGKXQLpmaZ6Hoxxf8hnwjiKuRfr&_nc_ohc=JOLe7xWSBQ8Ab5znhoj&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfB6ZdYtBoRO5JPij2Odg4qrbktzdRkAfdDl3phR0ZbD0g&oe=6622AF8C",
                                    "watermarked_video_sd_url": "",
                                    "watermarked_video_hd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/434152322_792637362202112_7786457532089703956_n.jpg?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGvmgGMjs7CcLWfbos_15bYgJOhCOiSfpmAk6EI6JJ-mbSyF0EYwBm3PLih-xNrmS9A8HTpIBlnWswRTE3jOjD7&_nc_ohc=-N2G8-IgN6MAb5RGug7&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfCNlRxjyLqZLBo4tH8vFws44jUyfsIC74AAFi5-qA6TJw&oe=6622A86B",
                                    "video_caption_urls": {
                                        "vi_VN": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.2093-6/434129084_396338889775549_7845431780490501963_n.srt?_nc_cat=103&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHVNSb80Kru3rpeL6dXp_ZgCIpdAM22nbUIil0AzbadtftV9sTtJW0bH5c_-QvE3KmLytku-qt5kQn2sT2Rcwul&_nc_ohc=kCw9HK8Mg_YAb5c1aCz&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfB15S-193BorFWc4kYbiVNhyKYklGYbHnDe2tk7X-6ArQ&oe=6622C7E7"
                                    }
                                }
                            ],
                            "creation_time": 1711422861,
                            "page_id": 107189848084236,
                            "page_name": "Trung Tâm Laptop Hải Phòng",
                            "page_profile_picture_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/434397572_1886829871737434_1169204249224867196_n.jpg?stp=dst-jpg_s60x60&_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEv8FXmy23RVrYtXOdHa1-dRxHDPWVtcPhHEcM9ZW1w-PXeGwz2HbV7YRXXMVD2DFWrvnSOByjpb7hsFli51ra6&_nc_ohc=9nWEaxmZZxYAb6016_N&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfAFihz5ZmyJTaelsT0MXmyWCQ1Bg5XHXq-HRtNLiAjymw&oe=6622A849",
                            "page_categories": {
                                "200600219953504": "Shopping"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Trung Tâm Laptop Hải Phòng",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.35426-6/434147393_950672066192557_8494083466041828065_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeF-55kappybjyrY6P5QNu_u8QEDsgO9i9vxAQOyA72L2zKOOSs0P55cH3FNxjioHb70zFjHUqvsBw67KoOkyvDy&_nc_ohc=iNuLcWz8kSIAb6eVR2d&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfCgeaYwDAW4tV0ECj3LQ-8O0eJr5xzTmR8Ncwny1vdRaQ&oe=6622DC57",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "✅ Surface Pro 5 ( i5 - 7200U / 8G / 256 SSD / màn 12&#039;5 2k Touch ) đáng mua nhất trong tầm giá #7trx #surfacepro5 #laptopcamung"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Trung Tâm Laptop Hải Phòng",
                            "disclaimer_label": null,
                            "page_like_count": 5502,
                            "page_profile_uri": "https://facebook.com/100091314824136",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712127600,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "933142758391094",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 1393885094827932,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "107189848084236",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Trung Tâm Laptop Hải Phòng",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120207917561720345",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "multi_images",
                            "title": null,
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": null,
                            "images": [
                                {
                                    "original_image_url": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.35426-6/435394262_1508724689710859_8463898651813113510_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGRc0c7OZTGtB2jMxv1BVnqh1xigAtCqteHXGKAC0Kq19-NgsZEAr4_FnOh_WpdifEM0N-2zYIDvYsEEe0RD9Ww&_nc_ohc=A8fypQ9r49YAb5rhHIP&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfBAOjgv3PaiE8SZIVQsIRxUqhyte0zAkKY74c-kg3DJnA&oe=6622B345",
                                    "resized_image_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/435309349_421515653810391_7389276238143267539_n.jpg?stp=dst-jpg_s600x600&_nc_cat=110&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeErKKIkyS9d3kkiq4OwpdDPpvmYSLjZ8Tum-ZhIuNnxO82H89ojEYwzSHhl2Mvsmt7-sdEm4ubfwX_AB1s2uEXB&_nc_ohc=K9o_OxorQNMAb55EyIy&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfBpLEUZMa4Xm0RSvg4Bh6bodZNdlLPQH9St_dKAnmpOsA&oe=6622DA0D",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-5.fna.fbcdn.net/v/t39.35426-6/435265952_1539801519898859_2388134115193273216_n.jpg?_nc_cat=104&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEWz-HBCXjH_E2-X8CBeZG7hJ6hu4LQ92eEnqG7gtD3Z47K47X1jeXZ7pqkBymmYfrpOndVPn4YtjIPq5uoZSiV&_nc_ohc=ZwS6MzjsTroAb71TXir&_nc_ht=scontent.fsgn2-5.fna&oh=00_AfBsl2WYnY4cXwO3rLhlBZ1NqRnW8r5kdEbDDqu1nG7EKg&oe=6622D949",
                                    "resized_image_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/435413535_1452594135653645_7685963390444122833_n.jpg?stp=dst-jpg_s600x600&_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHzg5_7toHcU90V4vIfEdCBosm-w_4o-6-iyb7D_ij7rx00Ro9LJoyf15SYtVfZY3oUDCJixtoDYAJB8SbBfVbE&_nc_ohc=5t32L5_mq48Ab6CAsi5&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfBnYwExlkLltHd6cAsdsdKnTiKEKkbCLThuYlmtqoPEYA&oe=6622AFCE",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/435250656_1336359707045352_3670114660837638093_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEfOQ2JyNGtfjGeCSgeodmRVNBbeamvwENU0Ft5qa_AQyC0N7pRItA0aYR60xmTCYEFiHVp0eg9NJ_MDUdAfOoO&_nc_ohc=tZ_Uk5r3KgEAb58bjcR&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfBVuPU4p5TNq8u6G9Z0coERimvxmoiZ-HYv3c-ql0j_SQ&oe=6622B1DE",
                                    "resized_image_url": "https://scontent.fsgn2-5.fna.fbcdn.net/v/t39.35426-6/435269401_408111848514695_4350129846838617636_n.jpg?stp=dst-jpg_s600x600&_nc_cat=104&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGfyjZrl4WP7uDdZVfZMrun3bWLBr6C7CndtYsGvoLsKeg5yPwJyr4UEj2T_aCUiq4tr8Ytnba1tP5LM3iKxQhr&_nc_ohc=qrhVqP8IzK8Ab6kFY3f&_nc_ht=scontent.fsgn2-5.fna&oh=00_AfBOzDPXumP1u5Ti28GIBAYYFOZAfYWu4kBwsVj0dST_Wg&oe=6622D7F1",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-5.fna.fbcdn.net/v/t39.35426-6/435323304_1524864441472788_454962922702236332_n.jpg?_nc_cat=104&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFVIocDHFycCSd1eunbzEanmPz1NpP2ENCY_PU2k_YQ0OsayZ8PfsypeIIUNMjCQS3ro8nBOT6vJbf4KC76qtG2&_nc_ohc=a3QhFUef67oAb5zJKqg&_nc_ht=scontent.fsgn2-5.fna&oh=00_AfApjeRR_KcJDwByXcHaGCTwP4Jmcwc3F8eK3Cxyoh4YZQ&oe=6622A8CE",
                                    "resized_image_url": "https://scontent.fsgn2-5.fna.fbcdn.net/v/t39.35426-6/435256764_1143789133721820_8338470962849165346_n.jpg?stp=dst-jpg_s600x600&_nc_cat=104&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHgutzOr_bG4Ri114LYYa3LkEpCMZOYaEuQSkIxk5hoS6b2ZN6bK742my1-AwLKK7H7HjSaygJajLUO0SMJmAfY&_nc_ohc=vp82aZCUoPYAb6IvX7g&_nc_ht=scontent.fsgn2-5.fna&oh=00_AfCGSZkAfJM3y4dD82s-ySMV0wwdIDRQGs-nz5TsMZFw-g&oe=6622D30D",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-5.fna.fbcdn.net/v/t39.35426-6/435268493_967352291690048_49591109168692933_n.jpg?_nc_cat=104&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeESRPJxiWyH9gCMn0IH-gv_UBMiYHbtVOFQEyJgdu1U4ci1gB0vwSxe_mu6d4ra5u2Poljjhfs52ybkxRIMa0wt&_nc_ohc=b1veOC67G4wAb6CA42j&_nc_ht=scontent.fsgn2-5.fna&oh=00_AfDCdLY7UzlBRUeWDLjMTLWOoC1HgVqTqtzDiXjh-Ca8Jw&oe=6622D784",
                                    "resized_image_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.35426-6/435298329_406476018767548_1782985665367139807_n.jpg?stp=dst-jpg_s600x600&_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEpsujdGKDYzqfqYVqWXcLDUxaglQpXgQNTFqCVCleBA42W02bd4usfjjFreRYL1wadimR1v4VrTPMI8DNzWGec&_nc_ohc=bufvnh731DAAb5oySUo&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDdprbVorSJDfGDzjK8IokXXGkr1iYyaqOVYRhIKMIzzg&oe=6622C303",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.35426-6/435251134_2293856120819283_6249765244098790976_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGfmB_F_RM3X6J-mBvz2rRGuiB7m0mU_5i6IHubSZT_mK1RJIf-ACnOBZeiceONOu878xpgP5IUFL7hu6gLfRVV&_nc_ohc=Z7Ef-eqYKNgAb4Kui-E&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfC331Jp6ED_gAtGKYsP088r9t8edOaqHRqV2sYZLIGpYQ&oe=6622C9D1",
                                    "resized_image_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.35426-6/435273783_2295451497313641_5834002369455212298_n.jpg?stp=dst-jpg_s600x600&_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEuTkyQeJ8KHtyW39_Gp5yBcwo9zy7N6sNzCj3PLs3qwyWBxnPP5G1rPi51JYarf_Xs7-_hrWLdImyv2TMn23F2&_nc_ohc=44xyGjr96DcAb7FbxOA&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfBVa5oIRKx4POY0GEHVxSeHiUauVfil6ExDp0nbWTqlVw&oe=6622DCE5",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/435229675_971267363921688_6346176407611294327_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGNsK8lZ1zrg9YNeCKkslr-GxhTieAAgssbGFOJ4ACCy1opsGnoZW1PIN8RiuuK1IiBDvTFVHRbd6XU7KDpxspA&_nc_ohc=LfBWT3cabwAAb4D-INv&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfBANQu2FqpT8DuslIhMfBXijh6oGBer4es-vNBT_AaCjg&oe=6622B7D0",
                                    "resized_image_url": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.35426-6/435312638_1417579535790024_441335510787944609_n.jpg?stp=dst-jpg_s600x600&_nc_cat=101&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHsm90esvh1AFe20CuPFwHstOCimbnFiry04KKZucWKvOkIeriuSaf0BmJaarjXtEOJIevDm2_3ooQBdg3AYTSb&_nc_ohc=RqcYpYdtGu0Ab6I0Q8z&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfDxBn5S1Hvyfih5eoYLvKmgvqHXTitUSVVhF859GPfmgQ&oe=6622C133",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/435239474_1077825380116223_364011276073716403_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGl7Rcr8fy4WuaDCoFNiU86rfd57RUYaMet93ntFRhox1haUEfroJD4yitXbPDSkENylUiDaj1XBplk34hCJNaP&_nc_ohc=6mL4sN5IWR4Ab4FC_J8&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfBRFaCzZGE0mrqmT8QUcJEFu-NvT_H2VeSXa1UCilmWzw&oe=6622D2EE",
                                    "resized_image_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/434410464_296925900095386_2397128945519252831_n.jpg?stp=dst-jpg_s600x600&_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFSWZTJy7m7nmIqft0mGyu4c4hjTDGggDpziGNMMaCAOkZ08APxE_VlOhGKf2giNksi5SsEJf0BEWuIbyDBR1HT&_nc_ohc=YmReUcYlhTkAb6IN6o4&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfD4vXBY8SX2_qxOHPGGLk_LdiggJWKqNmIOmvnQEK50hQ&oe=6622C2DA",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/435262751_940076757570217_1661259960382051505_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeH3LJyH7D2eCqSB3BdaYKHLmHdjJI039p2Yd2MkjTf2nSE8JjtzcRQ7UT5Ce_3wuXFM2EqBkY1X31RRa2EROPU4&_nc_ohc=tcweiAYktQ8Ab7CAsGX&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfCpg40W59XIx_zDUu1Z_DPex_CbJG5XULhIGRPC_j-TfA&oe=6622DBC9",
                                    "resized_image_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/435322801_1557830478406791_885956142455417214_n.jpg?stp=dst-jpg_s600x600&_nc_cat=106&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFFRThT4GLZQnrRu_3EGplTGwf1fmVeR5QbB_V-ZV5HlK4NzKxuk1q416HAO8vysmmNw9ipwRJWGmuudhr5c-EJ&_nc_ohc=A1pn_6Z_2AQAb7QlSCP&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfCqCsL1vCS0R01I4u5BNqDs0IL5xIp4oedfDFuxwLGE0w&oe=6622C531",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.35426-6/434417717_1547465809442531_8790458525926247598_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHqY8SI-WpU4ng2U7ZwSFXysXcG_qXvp76xdwb-pe-nvp87GzwA5sxC6IS76X3nEtChn7oWDMn1fp_wKcLdMqai&_nc_ohc=3YppgtUXpVEAb6p6WZV&_nc_oc=AdisncMm2oy7q9ZruPRrkS7yAlktewsJLzXEZgQX7KIeaWQoh5A3Ckvg4ppuyByMkGg&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfA2Q6mwKYgvWKwM5ravGx-feFTkMGshN5OfbL-kT_GbAg&oe=6622AAAA",
                                    "resized_image_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/435471908_241134845748775_1875452930025142663_n.jpg?stp=dst-jpg_s600x600&_nc_cat=110&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEai9gbfC6PYIc_tNPxIAhoBB5Q9LTZplwEHlD0tNmmXEX_v-_XEQsOyH0DR8TA5fmacJbA85YxOMmKwpjWztmA&_nc_ohc=YYUhXw4gqgYAb4MN3oe&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfDBh34-_ObxI3pw3a-53N1fyf8n9FyACiKnc8zSAc0ykw&oe=6622C8E5",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/435284479_815889657244428_5135002609226443950_n.jpg?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHwBIzIqX6eYkb3hTOZYpnkPu4cFF-IFi0-7hwUX4gWLZzrd7NcQst03w8PzZCAVX45mR-vgXPH4sb4tKxwKNtl&_nc_ohc=tY-ow-ST4zkAb6Q6VDK&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfCUnGDQNLAVIQXitJIylmM2HW17vQEVT7_yK7fk5_bKsA&oe=6622C0EF",
                                    "resized_image_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/435318711_311098691991708_1181995410320759609_n.jpg?stp=dst-jpg_s600x600&_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHUmmNdJtWeQ4aKFulr0SUgBSdhSiwkAkkFJ2FKLCQCSfH0LYztduFLA-KMFRazz9qQ1f3ZRsxDbEYNl4PSVqYx&_nc_ohc=zLQygmAcIV4Ab4aiPjk&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfA0u-z56omK4c13uGR6WTon319Hv-gOaN3zFoyLEYueZg&oe=6622A838",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/435229392_411109238321266_3926914636135812343_n.jpg?_nc_cat=100&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEBLww6OLcEns5tNrsr5OH04ir6K3veQdPiKvore95B05YrzOsGotb4uF13LT65MxJSxNravq3IyZVFglPLZu3H&_nc_ohc=TJ04n9rhxZkAb6dMiey&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfCzIEBOc45-5BWeS_1sy4wHYQTviExmDa_A_M6LWSTN6w&oe=6622ADBF",
                                    "resized_image_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/435229417_1598032434367797_5802712732928271947_n.jpg?stp=dst-jpg_s600x600&_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEEqzqlD9u_778mB0ncFwZ1HkWMLLeCj84eRYwst4KPzq33kFr6OnhWL3BGuZEQHfoS0vl3w45aLxXGRMkOhOSv&_nc_ohc=vDbzoLt-cfwAb7rRsQA&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfBVDEQZw3PhgpJ-k5ElokRQzGidk0nKw9HGnLdEOk4Yow&oe=6622B9E6",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/435240595_379819694965448_3089080376421901627_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHdnnM4jNQq2NDYKIdKgfZbMgCL023TaLcyAIvTbdNotwpejVwdCX3AMUzuAE8Tav1C-YLvgeTmkRrSa_0MO8GZ&_nc_ohc=B2wvMc4kgq0Ab4p_N56&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfDq6V6oHX3cm2D7Ywaasw6EeBJswUI0wtgSHhKJTLpzJQ&oe=6622BA4C",
                                    "resized_image_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/435480247_238700655937348_1535514550733748715_n.jpg?stp=dst-jpg_s600x600&_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHVlibY-w2o_lXvc6nWUUpgKZTVFM5DzP4plNUUzkPM_husrR0gBVu5L48aQKzNxp594jHw_DEYzihLOHUQkh_6&_nc_ohc=Z4kffNAzA_oAb66UcME&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfDdtct6vS_724jAAOOYk5wI-WmdXPuZvtG3rVHDbtDqcQ&oe=6622CB8D",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/435277683_339549845757672_5798608729395061064_n.jpg?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHrlv1DjMSj4Tomop4vuZBBn_AuYEbP746f8C5gRs_vju1SNAHP5jp__cJVwBNGaKtFN42WhGSlwkxP-HdRLDob&_nc_ohc=KFz098D3fH8Ab6I4GaK&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfD3_gbOjjUXFNT7FwBMQCdgjWsAj1CpXhLNbyXIRu_6DA&oe=6622ACE0",
                                    "resized_image_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/435346328_330920213324606_612245011175869772_n.jpg?stp=dst-jpg_s600x600&_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeH8yeHeYt3dYpVAPDjcmJKtMY9akeNkUT8xj1qR42RRP5csY_24hS_z7P1vU7SdrXdWcSDsH6StnYohg6ubxXYu&_nc_ohc=VhvMFlprbyYAb45U2YX&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfCp4EIbSoXxPVRhodyuAxyR-XFm-K58uVJ_GEIc1vPSVQ&oe=6622D7C2",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/435251134_1139900830771920_8450919585948663152_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeH261qx7caGDaq3ymMrsN2R2q1cpq_T4dvarVymr9Ph26NgWTOGQlFCU_UKmMl7yJ8LuK0xy-IM0MAThotCoADz&_nc_ohc=ytCRKj6bN2kAb7EaTvM&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfDkZSHVqL1UaT35F4iBEU9U7sa1ZGqqFQJDzyoV0lUIQA&oe=6622AC0A",
                                    "resized_image_url": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.35426-6/435261246_264736280034245_2996850935601791761_n.jpg?stp=dst-jpg_s600x600&_nc_cat=101&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEWzlAkWGAljSymRdVNFLxErHhg6UTnu0WseGDpROe7Re2x4Rawkt-cJjkOuXxtsandsUooMOMkk5zhRK23Q3DG&_nc_ohc=6DCcUMJGiIwAb4rAcoj&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfAQNotxOcwvNRa0kU0-U8UnxPpcxr8m3use-cdjbuFOGg&oe=6622CDC4",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/435287152_403028749027916_103241279505658524_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeF2AKX1BE3sDa98vaU53jOLH75qK9r1Coofvmor2vUKite6TxFNnntj6XXw84YAuJ4K3wy_XrIp92ZGFAqnKzW7&_nc_ohc=GTasXi9x_3QAb5KLMND&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfAwWepVbBhEn-k-MSnB3dZTcGXUzAgYQ6LW-Vnb2VIr3A&oe=6622DCB5",
                                    "resized_image_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/435250739_1112688903412961_5639301132759563280_n.jpg?stp=dst-jpg_s600x600&_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHBDwb4xHXCXMSTMloZuFnJkjZr_3VLerySNmv_dUt6vERwRro_8yVahG-D9zOg2wrYI4MMThlIsnqL6lWCBfs9&_nc_ohc=zCkzaoDv8i4Ab5cx2mV&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfCeNry4dJjlVP3TaRLMTW6vVeHK7QhOtQv-yQ4GcmoR9w&oe=6622D8C8",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.35426-6/435261659_919609069900749_4943099986990507224_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeF6yFg4VkProZYVtF7mB6nkQ5awC0C5jM9DlrALQLmMzyqNt72vl3X6Bm4aek0uRA60ya14q-Tp7v7Qle2L6Pz5&_nc_ohc=4etjFyfMWOkAb7drd-h&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfC-S1b3nAg_ulIsep40iwj7xSEC-dJvb6KKgN-1onj04g&oe=6622C504",
                                    "resized_image_url": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.35426-6/435261052_1626313044808091_7714713226368086040_n.jpg?stp=dst-jpg_s600x600&_nc_cat=101&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHV5_J7XijdLP6hhQDtcYoBxYneskVtZx7Fid6yRW1nHg7wtBkv5ASAjBAVAUo9jQPhS9qVTT4219l3a-r6Tq4g&_nc_ohc=XcGf_7nUzKgAb66kST0&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfBW3YczSQnQifL6Ada0pYCf-MckCFBiRM3NlHYqDLlI5Q&oe=6622CAE3",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/435273783_794673135875732_3078677545710049537_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFbYlBrGgFgouXGK87AyLRHOlq2R-Fl0Bc6WrZH4WXQF6BrXYNM5D914NjKVRlBgIJFOeqADwYag_FfkQ6aHbZE&_nc_ohc=TJqrpFcCI2IAb4XrMfT&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfB4s4RatZTvtaNaeQowAhG9Q-VXGr6qYcU-DXQI44EW3g&oe=6622C898",
                                    "resized_image_url": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.35426-6/435224004_782228366871957_4880809289860682117_n.jpg?stp=dst-jpg_s600x600&_nc_cat=101&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHoCc9eEmvdrYjdWLAHjy7bVvanT3juFqdW9qdPeO4Wp0XDBgLtgMXACliZ8SH_SzWH2CuTsYa0fKt6DdGXC2eV&_nc_ohc=MF90n5u2iv4Ab6xbfyl&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfBGckQ2oifMRvGRMywF2FfS5Sgd4SraWzMs1MGNZhEz5g&oe=6622D113",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/435259734_796710239022801_703615939063916353_n.jpg?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGHTVzY50Z-eH-G95QcpnJfh4gB49irIXuHiAHj2KsheyaecQF_BB0F8aLBI7WAQgfweC7e4Xgk57M3lI3afJpi&_nc_ohc=vtOXUFi3OoQAb7cqy2E&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfAdQYipjnn_RxFUze8yFMkgJivYPHHImq43A6tZwmsyjQ&oe=6622D45A",
                                    "resized_image_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/435237274_1462902071273273_1189452169804872691_n.jpg?stp=dst-jpg_s600x600&_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeG1O6ZmQ172JeNL22L3MF9os6D2qiZj-VazoPaqJmP5VviAt0doZqnoFtmX1evErdV9GOS2mBuC4NFULqCn3JT9&_nc_ohc=l8pd6sU5om4Ab6oWMtu&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfDl5Au8Ydth9LFvgp4FriEzHhytlZEF44cv6BDF9CsBYg&oe=6622C94C",
                                    "watermarked_resized_image_url": ""
                                }
                            ],
                            "videos": [],
                            "creation_time": 1712032930,
                            "page_id": 107189848084236,
                            "page_name": "Trung Tâm Laptop Hải Phòng",
                            "page_profile_picture_url": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.35426-6/435250240_262489003598975_5903997403817272096_n.jpg?stp=dst-jpg_s60x60&_nc_cat=101&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFPlwC1l2I-dUFa4wqIAl5A4KfTEIx0kCfgp9MQjHSQJ1tYI6_ertmqzz073pljWjGfITk3vDDcXgGcJ8lakj34&_nc_ohc=mNdXTt-A5DQAb5T3n2Z&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfA7xrjLeL5-416v4viIey4-a6nDAZh182-tmrY0ONsVgg&oe=6622D636",
                            "page_categories": {
                                "200600219953504": "Shopping"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Trung Tâm Laptop Hải Phòng",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-5.fna.fbcdn.net/v/t39.35426-6/435297890_346355397872271_6690876870218540183_n.jpg?_nc_cat=104&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFxHHiu_XVJ2rxr2-FN6jRZdyyxOlBaQgt3LLE6UFpCC1G0EwgmO3HQ5Td92-0U5bqhI5EpinnKfxHtcHsXR08d&_nc_ohc=LHY60zfm12IAb5YyDgA&_nc_oc=AdiJjLmVkNHWSsLXdLQARqhIEg-i_MwPg3s6Bt1u_NPxIGpubNSsjdCRXpsCf3jZ03s&_nc_ht=scontent.fsgn2-5.fna&oh=00_AfA7DpFQYd_T1TnnL-XaWMVC5eJY0quNJHI_q0u6huVWcw&oe=6622CC56",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "🙇‍♀️ 𝑯𝒂̉𝒊 𝑷𝒉𝒐̀𝒏𝒈 𝑪𝒐𝒎𝒑𝒖𝒕𝒆𝒓  xin chân thành cảm ơn quý khách hàng đã tin tưởng và lựa chọn ủng hộ #HPC trong suốt thời gian qua 🥰🥰<br /> ✨ Sự tin yêu của quý khách là động lực cho toàn thể công ty ngày càng phát triển và đưa tới những trải nghiệm dịch vụ tốt nhất tới tay khách hàng  🫶🫶<br /> ↪️ Ae inbox để được tư vấn ngay nhé !!!<br /> -------------------------------<br /> 𝑯𝒂̉𝒊 𝑷𝒉𝒐̀𝒏𝒈 𝑪𝒐𝒎𝒑𝒖𝒕𝒆𝒓 - 𝑻𝒉𝒆̂́ 𝒈𝒊𝒐̛́𝒊 𝒄𝒐̂𝒏𝒈 𝒏𝒈𝒉𝒆̣̂ 𝒕𝒂̣𝒊 𝑯𝒂̉𝒊 𝑷𝒉𝒐̀𝒏𝒈<br /> 🎁 Tặng ngay Combo Quà tặng or Voucher #200k<br /> ✨ Hỗ trợ trả góp ngay +Đổi mới 15 ngày đầu+Free phần mềm ,vệ sinh<br /> 🏡Địa chỉ : 82-84 Quán Nam, Kênh Dương, Lê Chân, Hải Phòng<br />  ☎ Hotline : 0981.919.595<br /> 🌍 Website : <a href=\"https://l.facebook.com/l.php?u=http%3A%2F%2Fmaytinhhaiphong.com%2F%3Ffbclid%3DIwAR0JUYsPhAxjqAu6Ks6PJwUFg71v4kfMosd_2S5qQzQmOSo_I16yxxdAtWc&amp;h=AT3k0wNe-BoDDYKkk81WRIOXw5rPneKup9cXGenXdv0Xg2h4_pZx_6Gt-axQehbgPbfod63W0gwn86-_YZCka3RjOfQms7uEosr_xdxw4LBEW6yVfM0Ywj41UkVD2t_vewj8c16ByQ\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">maytinhhaiphong.com</a>"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Trung Tâm Laptop Hải Phòng",
                            "disclaimer_label": null,
                            "page_like_count": 5502,
                            "page_profile_uri": "https://facebook.com/100091314824136",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712127600,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "366520452374277",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 1838942036544561,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "107189848084236",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Trung Tâm Laptop Hải Phòng",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120208303641360345",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "multi_images",
                            "title": null,
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": null,
                            "images": [
                                {
                                    "original_image_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/435262730_798806172158831_1611109001513060211_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHwEdGfk_EUUM9qjc-LHwJqu2fgoYeDNje7Z-Chh4M2N_9UlG4AMIujqgkRVRpUaAw2r8HFQWfd1j9KbDkYELg9&_nc_ohc=Hp-6CsYQRYYAb4zAO5D&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfCfW4_A4KGT2wX3Csj0Bhs6io4mIENZBm0mXaRcsQdboA&oe=6622B808",
                                    "resized_image_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/435505141_472284451791084_7534441955403697951_n.jpg?stp=dst-jpg_s600x600&_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEVO8c-O0PD7U89Ebc_UCLFN1Sku9aW0x03VKS71pbTHeUWS79m0LYOwDV1hk6cjB2W0iw2sfU9HYeZbD_nc80a&_nc_ohc=yIURdWlAqooAb6fUWSL&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfAQIMSD2wFmBmGJ-ocxiXZgivKeTZcgramUEC5RO7P-jw&oe=6622AA08",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/435502569_796601391911673_882371002967833024_n.jpg?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeE-BOj5A7rRBIlykqZGEMMC5CuILHGp8AvkK4gscanwC3jHT3WTSx2PduiRvu6RBUbuKY3hOH3hBnWfL66IvahN&_nc_ohc=CXF_6fdPRNoAb6W39tG&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfBRyAi0fqKfoK9vH6PBjAF-YexLrXURDFZ1gq5trOiy6A&oe=6622B5AB",
                                    "resized_image_url": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.35426-6/435512620_332888869415281_5712639234980589289_n.jpg?stp=dst-jpg_s600x600&_nc_cat=101&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeE77Op5-YJYOO-4_Sf5Yq0CYtCaY4fd1Xpi0Jpjh93Vem43e4JPkfibcNQSyqX3R0FxJc6Hc-BJ0J3Pwcq3YEmT&_nc_ohc=3KpzMaPabbUAb4vtgge&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfBsEKTY5iT3918cVj7JfEX81DrPhhlezvK4ejTsECys1A&oe=6622B65F",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.35426-6/437661517_398911089585357_2966844214593440494_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEJRiS4VlDOkNQ4YlSGx_htjiSGYbTI_2COJIZhtMj_YBbBcZZf1jpUMdTqgqA9B-9KWfmTU1_gSkKGzziLLo8t&_nc_ohc=4ae6y8Qge_4Ab51cYS0&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfD5JVVa4IymTDURat85GKlZMHnS1lpN19VIxcimsTpXNA&oe=6622D1D9",
                                    "resized_image_url": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.35426-6/435495646_1073204547105482_8724733665134899155_n.jpg?stp=dst-jpg_s600x600&_nc_cat=101&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGktF9O1E1wDQJ2ufFUBucdFsbg6cj6Hw8WxuDpyPofDzQtHv-TWYG91eAkzpnz7wYiWyknjQeOUBAjbpnc2Lne&_nc_ohc=lKnhrkCvBFQAb5abUfo&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfCPlHKttDX4HCNugc8iB5u4MZMKtmeXO2xA7ro2lwjo6w&oe=6622B67D",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/435499035_1399091154080229_8203764276420516555_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEnok4IiqDtyY38Pt2Os9sj1SDb7_pUcQzVINvv-lRxDDnDS7sC_C1t-YKldxSuSXRjqZ1X6BTR8B-WoRfB0jQu&_nc_ohc=buZaxfRevvYAb6SO2QD&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfBKEuGAYKf84EBF4Tu6s2FhHEPNNgDAFajC2n2a1yw5Jw&oe=6622D321",
                                    "resized_image_url": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.35426-6/435491010_1757727967971789_2000741995771043524_n.jpg?stp=dst-jpg_s600x600&_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGeIcsLczppjTOxH-cuyi6V9S8qqsweI5P1LyqqzB4jkw8hljPWE1cfskSazfkvxMxrW8uEBvf-KrcfJbdYfpW6&_nc_ohc=Mxio3xrxTV8Ab4RxtZr&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfC5Ome4fKvMa5Yx9-bGxLrx4QFxYMPShAr39FC4AdWYXQ&oe=6622BA3B",
                                    "watermarked_resized_image_url": ""
                                }
                            ],
                            "videos": [],
                            "creation_time": 1712804473,
                            "page_id": 107189848084236,
                            "page_name": "Trung Tâm Laptop Hải Phòng",
                            "page_profile_picture_url": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.35426-6/435512586_1094053068536454_2376305359743448314_n.jpg?stp=dst-jpg_s60x60&_nc_cat=101&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEAWbbtnl6feQqM_nKMstVNQuh-lF8APlRC6H6UXwA-VGnNsH_MmfZKE_pjzsLLqwe4oE1QJq66KEdY3LTO0RLA&_nc_ohc=Wh0ThGIwAfQAb4L1gW_&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfC3UzrEjDknNndSt5v5STugGnbQY6JUenTctZXoLORlPg&oe=6622B1C9",
                            "page_categories": {
                                "200600219953504": "Shopping"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Trung Tâm Laptop Hải Phòng",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/435509030_793377676024605_4905267758089189416_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeENJb1RlIYbOCqb8LZeH6p8FLFIvWFAGisUsUi9YUAaK7nBtqGezMrMnYDrlwNBrF-qocTx-lJi2A-Ypea4q0YO&_nc_ohc=RxMiOcRF1PAAb4mzvCZ&_nc_oc=AdiVRwbvr45d37H1fkbPaA02l3hZRWBV822pMWfLo7gUspnyEUZcKufAb71yJRi1Duc&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfDhpVO1aAJ4TWS_9IeEUZ_mn2lFN9g_DRzjZLqw2Ry_gQ&oe=6622D8E9",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "🔥 PC Gaming Siêu Mạnh, Giá Siêu Hời - Chỉ 𝟏𝟒.𝟗𝟗𝟎.𝟎𝟎𝟎 𝐕𝐍Đ! 🚀<br /> 📌 Cấu hình: 𝐈𝟓𝐠𝐞𝐧𝟏𝟐/ 𝐑𝐚𝐦 𝟏𝟔𝐆/ 𝐕𝐆𝐀 𝟐𝟎𝟔𝟎 𝟖𝐆𝐁 Chinh Phục Mọi Game - Sẵn Sàng Đối Đầu Mọi Thách Thức!<br /> -------------------------------<br /> ❌ CHỈ CÒN 10 COMBO tại #haiphongcom <br /> 🎁 Tặng kèm Combo phím chuột cao cấp<br /> 💵 Hỗ trợ TRẢ GÓP duyệt nhanh <br /> -------------------------------<br /> - Main h610 asus new  (bảo hành 36 tháng)<br /> - Cpu i5 12400f box new (bảo hành 36 tháng)<br /> - Ram 16gb d50 (2*8) DDR4 (bảo hành 36 tháng)<br /> - Vga PELADN RTX 2060 Super 8GB GDDR6 (bảo hành 36 tháng)<br /> - Ssd nvme 256gb (bảo hành 36 tháng)<br /> - Nguồn centaur Ct750w (bảo hành 36 tháng)<br /> - Vỏ titan trắng  + 7 fan led vô cực + tản khí centaur air02 ARGB (BH06T)<br /> ----------------------------------------------<br /> Ư𝐔 𝐃Ã𝐈 𝐊𝐇Ủ𝐍𝐆 𝐊𝐇𝐈 𝐌𝐔𝐀 𝐇À𝐍𝐆 𝐓Ạ𝐈 𝐇Ả𝐈 𝐏𝐇Ò𝐍𝐆 𝐂𝐎𝐌𝐏𝐔𝐓𝐄𝐑<br /> ✅ Miễn phí vệ sinh và bảo dưỡng máy tính trọn đời máy<br /> ✅Miễn phí bảo hành phần cứng tại nhà<br /> ✅Miễn phí đổi máy trong 1 tuần đầu nếu dùng máy không ưng ý hoặc muốn đổi lên cấu hình cao hơn.<br /> ✅Ngập tràn quà tặng đi kèm khi mua PC hoặc Laptop tại Hải Phòng Computer<br /> ✅Tất cả linh kiện máy tính đều nhập chính hãng, bảo hành lên đến 36 tháng.<br /> 👉HỖ TRỢ TRẢ GÓP:<br /> <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fhaiphongcomputer.vn%2Fhuong-dan-mua-tra-gop%2F%3Ffbclid%3DIwAR1NG-h5BONM6CqyxOPLFh69-h4_3eaFfX_UGDFidMUH__Y4z3ip408vPPc&amp;h=AT3rT4zg-RW5-GtA8NqmzZAw7V2PzwydF5bGvVyYi5WdN4UqD4NLN3LYSDr6eTkzhU6ZFbyujFrm_qCgXXb4gUgjwU1oqIyJSCcz4QgMBxmnSFXxLyAcPyvh3FzaQXmSQbumyL-UDg\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://haiphongcomputer.vn/huong-dan-mua-tra-gop/</a><br /> 👉CHÍNH SÁCH BẢO HÀNH:<br /> <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fhaiphongcomputer.vn%2Fchinh-sach-bao-hanh-san-pham...%2F%3Ffbclid%3DIwAR2SvyVDhoVYq7YWH-fNwyjYDJ9qUHyfKBxN3BnjDrprsthhicX93iu8qZ8&amp;h=AT3Ot8TVEful-zUKRinIM0_b_8RpcE24LsOeJ-Z7phRIpw8jg9JlSA4DbxQ04SOreLQFWbADls2TddW7ibnAyRzYChaQ2Aeep97fVsxcICdkiaJ_04BRH4XfpEKC3N5_0G9VTvpDpg\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://haiphongcomputer.vn/chinh-sach-bao-hanh-san-pham.../</a><br /> 👉CHÍNH SÁCH VẬN CHUYỂN:<br /> <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fhaiphongcomputer.vn%2Fchinh-sach-van-chuyen%2F%3Ffbclid%3DIwAR3cUkcL1D9-GiW6KqU194Z0kOdUeC9KTahwRx9rSofxH-QGNgxhU_bESK4&amp;h=AT1Bp1pc89QBiH_aPh6fN459b7KnsnHSt_bxA8CZ4Gtx6o13hpOsyrNhwZCnqkQC2vEdxJ8yZHeEY8oWXt9qE1mIVMuLfCFudRCAHWDs3Tn4wtYNVdgod7gNF-PGOb80l4RcAie3og\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://haiphongcomputer.vn/chinh-sach-van-chuyen/</a><br /> ====================<br /> Hải Phòng Computer chuyên PC Văn Phòng - PC ĐỒ HOẠ- Máy Xeon - PC Game Giá Rẻ - PC Tản Nhiệt Nước - PC AMD -Laptop<br /> ---------------------------------<br /> • Địa chỉ: 82,84 Quán Nam - Lê Chân - Hải Phòng<br /> • Hotline: 0981.919.595<br /> • Website: <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fhaiphongcomputer.vn%2F%3Ffbclid%3DIwAR1Ahzjl2lAtyBwWmEbqtR5kNY-eUSE2DA9mqEUfGN6mrWlreOW6wucs5bo&amp;h=AT2mLcYSJucMIU78MHSjfaUAOrG77zfaj4cm7YpzL_NWJ6tDXuK5tlcJumUJ1UOfwuIr2r785Hrf1H2uT8Ybu23KJVRf8dIiAifBSyLXRvlmzYKa2OUQdBn3IZJVWhwQxs__8BnGLg\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://haiphongcomputer.vn/</a><br /> • Tiktok: <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fwww.tiktok.com%2F%40haiphongcomputer.vn%3Ffbclid%3DIwAR1-G4RvVyKrCHeA4t-IWAvCibrIfhj3azpdzEu_HU80F6POFRr0tckppVg&amp;h=AT34JH0MUQ0YkZtUe8qPkTb5VoQ39y_6FKW8kJBnryoIpVVHz-qnOtEgxmnIlpS6gEw8gRwR7UvKjEvalQed-qz5AvLFc3eaMgmvnrm-NoBRabtqJomrTUX_b6hsJcomC0IXRCpweg\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://www.tiktok.com/&#064;haiphongcomputer.vn</a><br />  #PCGaming #SiêuKhuyếnMãi"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Trung Tâm Laptop Hải Phòng",
                            "disclaimer_label": null,
                            "page_like_count": 5502,
                            "page_profile_uri": "https://facebook.com/100091314824136",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712732400,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "2745185798967379",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 3639721482953976,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "107189848084236",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Trung Tâm Laptop Hải Phòng",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120207917229530345",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "multi_images",
                            "title": null,
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": null,
                            "images": [
                                {
                                    "original_image_url": "https://scontent.fsgn2-5.fna.fbcdn.net/v/t39.35426-6/434884205_968082138275786_672299885941658286_n.jpg?_nc_cat=104&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEKhVFJUpeLu1d4SRg1b5tteo2Uo3sGP8h6jZSjewY_yCCMJhiJSSkdBGT_Yy1Lm7Oh7kVVjY56CZJ2L4Rl3xTP&_nc_ohc=Cei5cXcIiYwAb4DUKZI&_nc_ht=scontent.fsgn2-5.fna&oh=00_AfDkytju2eDhhJxKBHl3XY8-jtVqs87vqE5KK0cU5oLQyA&oe=6622B2A0",
                                    "resized_image_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/434922174_773505414746901_2958820823393337438_n.jpg?stp=dst-jpg_s600x600&_nc_cat=100&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGT444vJe7sM0F-tkJ3JEUfzS3XWOA8gAnNLddY4DyACbjaVAH548mfNpXyPeAOpTxv57E5fLE08fG3O1b3gQWu&_nc_ohc=8McZlXZsmmEAb76eFnI&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfCJJ51gNz9qGNHuwvUH27Aatl1zBmFmyQIGVJ16CahdgQ&oe=6622B34F",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.35426-6/434923505_1144555526700394_4372121218087170152_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHFtzIP0uL6-XP2qO3ymNnF-x0xEAqiX6D7HTEQCqJfoEdvYB5HHNjNf1w-GwqEeo_ja2zYbsCIaN2l9KIqHXK8&_nc_ohc=3gHdSfKvKuMAb4vkbCU&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfCXzmgv3HhBdWwJXBellwj0C5NJwAKIgeg5o4AsCbX4QQ&oe=6622D246",
                                    "resized_image_url": "https://scontent.fsgn2-5.fna.fbcdn.net/v/t39.35426-6/434910178_1359383768089583_6526018260331572300_n.jpg?stp=dst-jpg_s600x600&_nc_cat=104&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFvkkHKPHw5lrSfqjboEkc7na7rB51MSMedrusHnUxIx7tgCsr9-gU6ZCIRTWH2SjI7ykC0W3eeqLE5fhq3MiXG&_nc_ohc=qpXmuSLrrX8Ab6x-6PC&_nc_ht=scontent.fsgn2-5.fna&oh=00_AfBLbDVUoyXTXNKqNVlJFZzrisJ85PdzkBmVBqCq4BC9_Q&oe=6622A55B",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/434926559_2760984490742482_606848115972054784_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEcM1lFls-B6lNpuDeFLcq1bXOBBdetQyxtc4EF161DLLlHdfy41jxQr7m8kqlbDCfvaNUWDCTyo-C10A7IVU5w&_nc_ohc=x_Dh_5G2KtEAb7VeemB&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfD8fTH5VPzGQa8YOTc1r1QwHAKGkeCfs-cMbVunYX0srA&oe=6622A56F",
                                    "resized_image_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.35426-6/434922228_1359893564716848_3552347092723181761_n.jpg?stp=dst-jpg_s600x600&_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEOIrsxC5j2Sh43aNg6xkR4yIK9HOSKBX3Igr0c5IoFfSYJqtqXkAKRNhWCVm-gwwMgpiPCjREDvGD0GoF6ZUan&_nc_ohc=owoIeC96d0cAb729A2E&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfCR37i0bgzohKCK0-AnAKXkL5-52pkUakUn4PMFdXjRnA&oe=6622D2E5",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.35426-6/434940237_922151619609068_8626407284045946702_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEfh7Ji0DnMe2cPi3mb2GWVm7go5YP6ZTKbuCjlg_plMurM4CcLeWVTfBXYdwLY3pbVhtd0Di0r_c-OuyQNRb7t&_nc_ohc=R0oY1tDz33IAb5K0xaN&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfAyDGAwFJjZgELQ9w2dvnuFbh90_adh2VmDJvYVzyNSGA&oe=6622DAF0",
                                    "resized_image_url": "https://scontent.fsgn2-5.fna.fbcdn.net/v/t39.35426-6/434953547_339649512433429_4496925302504211931_n.jpg?stp=dst-jpg_s600x600&_nc_cat=104&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHjrQxpI9qfbFq9y8YAI6DFlqweLfBZ0R6WrB4t8FnRHkfCkHJRxnYvoZl7LF6TFK3m7wlXgOj1NL0YBpXLN_C1&_nc_ohc=NtEwjxuqHCoAb5xuJz_&_nc_ht=scontent.fsgn2-5.fna&oh=00_AfB4Pow0zmEimTpSSz8a95Mq1eQ3JcYhmq6ivzzay_-FSg&oe=6622C9F6",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/434910139_1164034504511989_3783632943716116268_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGJV6kytF1Z455FTTvFJtKT0Es0AT3N7eDQSzQBPc3t4EKEqoBTE0vn5rh1A7U6Ch_dekTsK-NbtyVy4rYwph6z&_nc_ohc=BHX9R88fwZgAb7vx5F6&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfCzo4-JbSBKWlaqwyQ6RRwJbZOGcQVttsRFg2prQsyCxA&oe=6622CCA8",
                                    "resized_image_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/434887252_3673212646300576_7037516468309344338_n.jpg?stp=dst-jpg_s600x600&_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEoTIPXKlst7Yj-U3KHLGMZWe4yl32apj9Z7jKXfZqmP5NC0Ol5bIyJnGGxpfybmkBBo3ySXkeG8G0oeO1yusdA&_nc_ohc=8lHOhlSqOQ8Ab5fSkYo&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfCQnwZQA4ya37hoNUmu_5fsGmuBk6lKPtUnuIf6zHWaOQ&oe=6622C5D5",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/434975827_1816550312173538_3371891376164464754_n.jpg?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFzz2rAPaHanqdbN8gi85uMMYc5bgtu9GwxhzluC270bAjfvP5weWyT9Ce2jf5TH7-bIyov3pTFaE6W6IeUkJo4&_nc_ohc=7XjQVIfgO04Ab70cmBk&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfAMuEl9Eba3QOOm1j6QWqgvF5pa0SEERYQVxMMcvHlSnA&oe=6622DABE",
                                    "resized_image_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.35426-6/434956042_324252413633100_3179568707340590634_n.jpg?stp=dst-jpg_s600x600&_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeF2sPxXlLeK6bxQAQO62SKluUH-Y9UBrmC5Qf5j1QGuYKmT04I_Wq6f__GStqRK4npHoKPgfQXIlgfuqSCb3k2s&_nc_ohc=P2YOEFxi7J0Ab5vm-Gu&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDtBFlAJXIRWCEB7lO_ANCgkzCNvDmOszcnSe5DtDhjaA&oe=6622C427",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.35426-6/434959893_1155484452020155_4993618911173270392_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHcQ2srmkd1_N4Z0siUKbVsZyHyoD1QZCFnIfKgPVBkIUT9UUZZdwSB-vhbvZoaNQrB5fwkHFXqh-Np2DjjYckp&_nc_ohc=uqNFl-4ChNEAb5TIGNu&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfB7q1X9c-jMo0XlzPzT6cSAHqggvUtXdhiHHffRIo_55g&oe=6622A693",
                                    "resized_image_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/434961448_381671414709398_4402285234890939254_n.jpg?stp=dst-jpg_s600x600&_nc_cat=103&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGh59dvQ4gNqmmnJdIPUKeKiwHwl4tiV8CLAfCXi2JXwJ63IGjFS5sNPFHU2uwRjIaPTbVT1lNQNbV5eVoBBzMj&_nc_ohc=nzIgAAhIAm8Ab4vKoqu&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfCkNn3Mpyzi-6zzkQyulWi5HrAC59110ivQa0hfh3773A&oe=6622C032",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/434952165_825497786062305_2604207969843596723_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGG1m6ovv2u_y1UD-iyEOPTTY2KLB9IiztNjYosH0iLO1EUv72427TUayrDBAWcMb9TOze-NWbdI3V2XoJkZ4GC&_nc_ohc=GhUnYu5vlQAAb5WnUHJ&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfAxvSMjj-SfYwR76CXiubIRCC0tNxtEdW8u2UnP5BvczA&oe=6622CA9D",
                                    "resized_image_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/434928514_1471512160145042_5303507824770566022_n.jpg?stp=dst-jpg_s600x600&_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEs4PVsX4tUNUF590eZQZB8BoIJCwEtKq8GggkLAS0qr_VikrFQDOp1MFJoUTHJj3ChE-SUC96K4pMEBXT4y3Lv&_nc_ohc=05pHM6ztS8gAb4VQNXm&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfCSeqTYVdOyyAkEfTEIyLQQg_dREUwwylsrW2f2k_93WA&oe=6622CE24",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/435062369_380870214927643_4899857613818727615_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHD1GkyzNQRYk1Yswq8prnq0SIaer-cY1DRIhp6v5xjUM3RRRBs7BVYgm1bUCWx6tlJmT5TsnJEHDxuZ62i5wKd&_nc_ohc=xHvLt75AmMEAb6QrhkV&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfDgHgKufsAhwNW0Dq9w9S5y_DgtDYI1qS4KAcc0rOedMw&oe=6622B9A6",
                                    "resized_image_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/434947981_958208842571337_8475677076436773438_n.jpg?stp=dst-jpg_s600x600&_nc_cat=106&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeECATel5HZZgsMm6e1TC78qEE3CMABaD-AQTcIwAFoP4BU5e2MNwFE5TWWm0-wgXjeuwMgKil4Pc3enW0K06G9Q&_nc_ohc=C27naP1avWEAb6D-VBc&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfApMUr4K1kdHqj5Diov9gDqC-jEOS5BLtENOP4Iam3ClA&oe=6622BCA3",
                                    "watermarked_resized_image_url": ""
                                }
                            ],
                            "videos": [],
                            "creation_time": 1712032313,
                            "page_id": 107189848084236,
                            "page_name": "Trung Tâm Laptop Hải Phòng",
                            "page_profile_picture_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.35426-6/434945296_385643707714785_1147359391341855825_n.jpg?stp=dst-jpg_s60x60&_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFICpQrV51jFrpp1kbeaIP9xGeaDR2dR97EZ5oNHZ1H3pHprHsYRar-p8pvxdqNoJ8LA4ZvviiiEd831i3BmxYE&_nc_ohc=1Px_5_5JCYgAb7Q7eaO&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDzV2IIOgQz1HqEz7GEf39VZ58hiS0xl-e5eXnLlbZFIg&oe=6622BFDD",
                            "page_categories": {
                                "200600219953504": "Shopping"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Trung Tâm Laptop Hải Phòng",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/434881055_3340353582924356_7532911685355478441_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFqigHo3F7y5t6ZTswIG4GfyIVku7CgOoDIhWS7sKA6gLR5MdES1Lsu9ie_nAl8CutdffpXWwivkdYYZPPnmgg4&_nc_ohc=18Gcd3W1-AQAb6_5K1J&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfC_563xQA1MLhDYecc53ukCpoUmGT9GDIt_iCaNNumwRQ&oe=6622DBE5",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "🎁 𝐔̛𝐮 Đ𝐚̃𝐢 𝐓𝐡𝐚́𝐧𝐠 𝟒 - 𝐐𝐮𝐚̀ 𝐓𝐚̣̆𝐧𝐠 𝐂𝐡𝐚̂́𝐭 𝐋𝐮̛̀  -𝐕𝐨̀𝐧𝐠 𝐪𝐮𝐚𝐲 𝐦𝐚𝐲 𝐦𝐚̆́𝐧 𝐜𝐡𝐨̂́𝐭 𝐧𝐠𝐚̀𝐧 𝐪𝐮𝐚̀ 𝐭𝐚̣̆𝐧𝐠🎁<br /> 💁‍♀️ Mua sắm PC, Laptop thả ga, không lo về giá! Trong tháng 4 này, HPCOM hân hạnh mang đến chương trình ưu đãi đặc biệt. Khi quý khách hàng mua trọn bộ PC hoặc laptop, bạn sẽ được tham gia vào chương trình vòng quay may mắn với những phần quà hấp dẫn sau:<br /> 🎉 Các Phần Quà Hấp Dẫn:<br /> - Bàn phím Lightning AD7700s + Chuột Coolerplus FC112 led + Lót chuột 80.30<br /> - Bàn phím Dareu cơ không dây EK810G đen + Mô hình Thanh Gươm Diệt Quỷ<br /> - Phiếu giảm giá trực tiếp 300k<br /> - Tai nghe T39 + Mô hình Rengoku<br /> - Combo 4 Fan RGB + Hub điều khiển + Lót chuột 80.30<br /> - Combo Balo + Chuột và Lót chuột<br /> - Loa Bluetooth L30 + Đế tản nhiệt Laptop kim loại<br /> <br /> 🎁 Điều Kiện Áp Dụng:<br /> Các phần quà trên chỉ áp dụng khi quý khách mua trọn bộ PC hoặc laptop tại HPC trong tháng 04 này.<br /> Đừng chần chừ nữa! Hãy đến với HPC ngay để không chỉ sở hữu những sản phẩm chất lượng mà còn có cơ hội nhận ngay những phần quà hấp dẫn.<br /> ------------------------------------<br /> 💎 𝑳𝒊𝒔𝒕 𝑳𝒂𝒑𝒕𝒐𝒑 𝒗𝒂̆𝒏 𝒑𝒉𝒐̀𝒏𝒈 𝒄𝒖̃ <br />  💻𝐋𝐀𝐏𝐓𝐎𝐏 𝐃𝐄𝐋𝐋 𝐋𝐀𝐓𝐈𝐓𝐔𝐃𝐄 𝟕𝟐𝟖𝟎: I5-7300U/ 8GB/ 256g SSD #5tr500<br />  💻𝐋𝐀𝐏𝐓𝐎𝐏 𝐃𝐄𝐋𝐋 𝐋𝐀𝐓𝐈𝐓𝐔𝐃𝐄 𝟕𝟒𝟕𝟎: I5-6300U/8GB/ 256g SSD #5tr290<br />  💻𝐋𝐀𝐏𝐓𝐎𝐏 𝐇𝐏 𝐄𝐋𝐈𝐓𝐄𝐁𝐎𝐎𝐊 𝟖𝟒𝟎 𝐆𝟓: I5- 8350U/8GB/ SSD 256g #6tr590<br /> <br /> 💻 𝐋𝐀𝐏𝐓𝐎𝐏 𝐃𝐄𝐋𝐋 𝐋𝐀𝐓𝐈𝐓𝐔𝐃𝐄 𝟕𝟒𝟗𝟎: I5-8350U/ 8GB/ 256g SSD #6tr490<br /> 💻𝐋𝐀𝐏𝐓𝐎𝐏 𝐃𝐄𝐋𝐋 𝐈𝐍𝐒𝐏𝐈𝐑𝐎𝐍 𝟕𝟒𝟕𝟐: I5-8250U/8GB/ 256g SSD/MX150 #7tr900<br /> 💻 𝐋𝐀𝐏𝐓𝐎𝐏 𝐇𝐏 𝐄𝐋𝐈𝐓𝐄𝐁𝐎𝐎𝐊 𝟏𝟎3𝟎 𝐆3: I5-8350U/ 8GB/ 256g SSD #8tr800<br />  💻𝐒𝐔𝐑𝐅𝐀𝐂𝐄 𝐏𝐑𝐎 𝟓 : I5 – 7200U / 8GB : SSD 256GB/ 12.5 ‘’ 2K #7tr290<br />  💻𝐋𝐀𝐏𝐓𝐎𝐏 𝐃𝐄𝐋𝐋 𝐗𝐏𝐒 𝟗𝟑8𝟎 : I5-8350U/ 8GB/ 256g SSD #9tr490<br />  💻𝐌𝐀𝐂𝐁𝐎𝐎𝐊 𝐀𝐈𝐑 𝟐𝟎𝟏𝟖 : I5 /8GB/ 256g SSD #9tr500<br /> 💎 𝑳𝒊𝒔𝒕 𝑳𝒂𝒑𝒕𝒐𝒑 𝒗𝒂̆𝒏 𝒑𝒉𝒐̀𝒏𝒈 𝒎𝒐̛́𝒊<br />  💻𝐒𝐔𝐑𝐅𝐀𝐂𝐄 𝐋𝐀𝐏𝐓𝐎𝐏 𝟒 : I5 – 1135G7/ 8GB / SSD 512g #14tr490<br /> <br /> 💻 𝐋𝐀𝐏𝐓𝐎𝐏 𝐃𝐄𝐋𝐋 𝐈𝐍𝐒𝐏𝐈𝐑𝐎𝐍 𝟑𝟓20: I5-1135G7/8GB/ 256g SSD #11tr500<br /> 💻 𝐋𝐀𝐏𝐓𝐎𝐏 𝐃𝐄𝐋𝐋 𝐈𝐍𝐒𝐏𝐈𝐑𝐎𝐍 𝟑𝟓20: I5-1235U/16GB/ 512g SSD #12tr990<br /> <br /> 💻 𝐋𝐀𝐏𝐓𝐎𝐏 𝐃𝐄𝐋𝐋 𝐈𝐍𝐒𝐏𝐈𝐑𝐎𝐍 𝟓𝟔𝟐𝟎 : I5-1240P/16GB/ 512g SSD #14tr790<br />  💻𝐋𝐀𝐏𝐓𝐎𝐏 𝐃𝐄𝐋𝐋 𝐈𝐍𝐒𝐏𝐈𝐑𝐎𝐍 𝟕𝟒𝟑𝟓 : R5-7535U/8GB/ 512g SSD #13tr790<br />  💻𝐋𝐀𝐏𝐓𝐎𝐏 𝐃𝐄𝐋𝐋 𝐈𝐍𝐒𝐏𝐈𝐑𝐎𝐍 𝟓𝟒𝟐𝟎 : I5-1240P/16GB/ 512g SSD #15tr200<br />  💻 𝐋𝐀𝐏𝐓𝐎𝐏 𝐃𝐄𝐋𝐋 𝐈𝐍𝐒𝐏𝐈𝐑𝐎𝐍 𝟓𝟔𝟑𝟎 : I5-1340P/16GB/ 512g SSD #17tr000 <br />  💻𝐋𝐀𝐏𝐓𝐎𝐏 𝐃𝐄𝐋𝐋 𝐈𝐍𝐒𝐏𝐈𝐑𝐎𝐍 𝟓𝟑𝟑𝟎 / i5-1340P/16GB/ 512g SSD #17tr990<br /> 💎 𝑳𝒊𝒔𝒕 𝑳𝒂𝒑𝒕𝒐𝒑 𝑮𝒂𝒎𝒊𝒏𝒈<br />  💻𝐋𝐀𝐏𝐓𝐎𝐏 𝐇𝐏 𝐆𝐀𝐌𝐈𝐍𝐆 𝐕𝐈𝐂𝐓𝐔𝐒 𝟏𝟓/ R5- 7535HS/8GB/ SSD 512g /GTX 2050 4G #15tr490<br />  💻𝐋𝐀𝐏𝐓𝐎𝐏 𝐃𝐄𝐋𝐋 𝐆𝐀𝐌𝐈𝐍𝐆 𝐆3 3590 /I5-6600H/8GB/ 512g SSD/RTX 3050 4G #18tr500 <br />  💻𝐋𝐀𝐏𝐓𝐎𝐏 𝐀𝐂𝐄𝐑 𝐍𝐈𝐓𝐑𝐎 𝟓 𝟐𝟎𝟐𝟏 𝐀𝐍𝟓𝟏𝟓-𝟓𝟕 / I7-11800H/16GB/ 512g SSD/RTX 3050 4gb #15tr990 <br />  💻𝐋𝐞𝐧𝐨𝐯𝐨 𝐆𝐚𝐦𝐢𝐧𝐠 𝐋𝐎𝐐 𝟏𝟓𝐈𝐇𝐑𝟖 / i5 13420H/ 8GB/ 1T SSD/RTX 3050 6gb #19tr500 <br /> 💻𝐋𝐞𝐧𝐨𝐯𝐨 𝐥𝐞𝐠𝐢𝐨𝐧 𝟓 𝐑𝟕-𝟕𝟖𝟒𝟎𝐇/𝟏𝟔𝐆/𝐬𝐬𝐝 𝟓𝟏𝟐/𝐑𝐓𝐗 𝟒𝟎𝟔𝟎 𝟖𝐆 #24tr990<br /> <br />  ----------------------------------<br /> &gt;&gt;&gt; Cấu hình 1 <br /> - Main  H81  ( bảo hành 24 tháng)<br /> - Cpu G3220 likenew ( bảo hành 24 tháng)<br /> - Ram 8g ddr3 ( bảo hành 36 tháng)<br /> - Nguồn Polima ( bảo hành 18 tháng)<br /> - SSD 120gb ( bảo hành 36 tháng)<br /> - Vỏ văn phòng <br /> Giá: 2.700.000<br /> Trả trước: 1.080.000<br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 2<br /> - Main H81 ( bảo hành 24 tháng)<br /> - cpu i5 4570 like new ( bảo hành 12 tháng)<br /> - Ram 8g ddr3 ( bảo hành 36 tháng)<br /> - Nguồn Centaur 350w ( bảo hành 36 tháng)<br /> - Ssd 120gb ( bảo hành 36 tháng)<br /> - Vỏ văn phòng<br /> Giá: 3.399.000<br /> Trả trước chỉ từ: 1.360.000<br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 3<br /> -Main H310 tm ( bảo hành 06 tháng)<br /> - Cpu G5400 tm ( bảo hành 06 tháng)<br /> - Ram 8g ddr4  tm ( bảo hành 06 tháng)<br /> - SSD 240gb New ( bảo hành 36 tháng)<br /> - Nguồn 350W tm ( bảo hành 06 tháng)<br /> - Vỏ Văn Phòng<br /> GIá: 3.099.000<br /> Trả trước: 1.240.000<br /> -------------------<br /> &gt;&gt;&gt;  Cấu hình 4<br /> - Main Asus/ MSI/ gigabyte H410 ( bảo hành 36 tháng)<br /> - Cpu G5905 ( bảo hành 36 tháng)<br /> - Ram 4g ddr4 ( bảo hành 36 tháng)<br /> - Nguồn Vp480 ( bảo hành 18 tháng)<br /> - SSD 120gb ( bảo hành 36 tháng)<br /> - Vỏ Văn Phòng<br /> Giá: 4.699.000<br /> Trả trước: 1.880.000<br /> -------------------<br /> &gt;&gt;&gt;  Cấu hình 5<br /> - Main MSI H510M-b ( bảo hành 36 tháng)<br /> - Cpu G5905 ( bảo hành 36 tháng)<br /> - Ram 8g ddr4 ( bảo hành 36 tháng)<br /> - Nguồn Centaur 350w ( bảo hành 36 tháng)<br /> - SSD  240gb ( bảo hành 36 tháng)<br /> - Vỏ văn phòng<br /> Giá: 4.950.000<br /> Trả trước: 1.980.000<br /> --------------------<br /> &gt;&gt;&gt;  Cấu hình 6<br /> - Main MSI H510M-b ( bảo hành 36 tháng)<br /> - Cpu G5905 ( bảo hành 36 tháng)<br /> - Ram 8g ddr4 ( bảo hành 36 tháng)<br /> - Nguồn Centaur 350w ( bảo hành 36 tháng)<br /> - SSD br nvme 128g ( bảo hành 36 tháng)<br /> - Vỏ văn phòng<br /> Giá: 4.799.000<br /> Trả trước: 1.920.000<br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 7<br /> - Main H81 ( bảo hành 24 tháng)<br /> - cpu i5 4570 ( bảo hành 12 tháng)<br /> - Ram 8g ddr3 ( bảo hành 36 tháng)<br /> - Nguồn Centaur 350w ( bảo hành 36 tháng)<br /> - SSD 240gb ( bảo hành 36 tháng)<br /> - Vỏ văn phòng<br /> Giá: 3.600.000<br /> Trả trước :1.440.000<br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 8<br /> - Main Asus/giga/ MSI H410M  ( bảo hành 36 tháng)<br /> - Cpu i3 10105 ( bảo hành 36 tháng)<br /> - Ram 4g ddr4 ( bảo hành 36 tháng)<br /> - Nguồn Vp480 ( bảo hành 18 tháng)<br /> - SSD 120gb ( bảo hành 36 tháng)<br /> - Vỏ văn phòng<br /> Giá: 5.790.000<br /> trả trước: 2.316.000<br /> ---------------------<br /> &gt;&gt;&gt; Cấu hình 9<br /> - Main MSI H510M  pro ( bảo hành 36 tháng)<br /> - Cpu i3 10105 ( bảo hành 36 tháng)<br /> - Ram 8g ddr4 buss 2666 ( bảo hành 36 tháng)<br /> - SSD 240gb  ( bảo hành 36 tháng)<br /> - Nguồn Centaur 350W ( bảo hành 36 tháng)<br /> - Vỏ văn phòng<br /> Giá: 6.550.000<br /> Trả trước:2.620.000<br /> <br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 10<br /> - Main MSI H510M pro ( bảo hành 36 tháng)<br /> - Cpu i5 10400 ( bảo hành 36 tháng)<br /> - Ram 8g ddr4 buss 2666 ( bảo hành 36 tháng)<br /> - SSD 240g  ( bảo hành 36 tháng)<br /> - Nguồn Centaur 350w ( bảo hành 36 tháng)<br /> - Vỏ văn phòng<br /> Giá:7.450.000<br /> Trả trước: 2.980.000<br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 11 <br /> - Main MSI H510M pro ( bảo hành 36 tháng)<br /> - Cpu i5 10400 ( bảo hành 36 tháng)<br /> - Ram 8g ddr4 buss 2666 ( bảo hành 36 tháng)<br /> - SSD nvme 128g ( bảo hành 36 tháng)<br /> - Nguồn Centaur 350w ( bảo hành 36 tháng)<br /> - Vỏ văn phòng<br /> - Thiết bị thu wifi + blutooth Asus ax3000 ( bảo hành 36 tháng)<br /> Giá:7.999.000<br /> Trả trước: 3.200.000<br /> <br /> &gt;&gt;&gt; Cấu hình 12<br /> - Main H610M ( bảo hành 36 tháng)<br /> - Cpu i5 12400 ( bảo hành 36 tháng)<br /> - Ram 16gb ddr4 8*2 Buss 2666 ( bảo hành 36 tháng)<br /> - Nguồn Centaur 450w 80 plus ( bảo hành 36 tháng)<br /> - SSD 120gb ( bảo hành 36 tháng)<br /> - HDD 1T ( bảo hành 24 tháng)<br /> - Vỏ văn phòng<br /> Giá: 10.199.000<br /> Trả trước: 4.080.000<br /> -------------------<br />  𝐂𝐚̂́𝐮 𝐡𝐢̀𝐧𝐡 𝐜𝐡𝐨̛𝐢 𝐠𝐚𝐦𝐞 𝐋𝐨𝐋, 𝐅𝐢𝐟𝐚, Đột 𝐤𝐢𝐜𝐡, 𝐂𝐬𝐠𝐨,...<br /> &gt;&gt;&gt; Cấu hình 13 <br /> - Main h81 (bảo hành 24 tháng)<br /> - CPU I5 4570 ( bảo hành 06 tháng)<br /> - Ram 8g ddr3  (bảo hành 36 tháng)<br /> - Ssd 240gb (bảo hành 36 tháng)<br /> - Vga 730 2g ddr5 (bảo hành 36 tháng)<br /> - Nguồn 350w (bảo hành 06 tháng)<br /> - Vỏ văn phòng<br /> Giá:4.799.000<br /> trả trước: 1.920.000<br /> --------------------<br /> &gt;&gt;&gt; Cấu hình 14<br /> - Main H110 ( bảo hành 24 tháng)<br /> - cpu i5 6400 ( bảo hành 12 tháng)<br /> - Ram 8g ddr4 ( bảo hành 36 tháng)<br /> - Nguồn Centaur 350w ( bảo hành 36 tháng)<br /> - Ssd 120gb ( bảo hành 36 tháng)<br /> -Card 750ti 4g (BH 24th)<br /> - Vỏ xigmatek XA20<br /> Giá:5.599.000<br /> Trả trước 2.240.000<br /> -----------------------<br /> &gt;&gt;&gt; Cấu hình 15 &quot; chơi lol, fifa, csgo&quot;<br /> Main H81 ( bảo hành 24 tháng)<br /> Cpu i5 4570 ( bảo hành 06 tháng)<br /> Ram 8g ( bảo hành 36 tháng)<br /> nguồn 450w 80plus ( bảo hành 36 tháng)<br /> VGa 1060 3g ( bảo hành 06 tháng)<br /> SSD 240gb ( bảo hành 36 tháng)<br /> Vỏ văn phòng<br /> Giá: 5.599.000<br /> Trả trước: 2.240.000<br /> -----------------------<br /> &gt;&gt;&gt; Cấu hình 16 ( giả lập, render, chơi game hot)<br /> - Mainboard X99( bảo hành 06 tháng)<br /> - cpu E5 2680 V4  ( bảo hành 06 tháng)<br /> - Ram SKhynix 16G DDR4 2133 ( bảo hành 06 tháng)<br /> - Nguồn Centau 450w ( bảo hành 36 tháng)<br /> - Ssd nvme 128g ( bảo hành 36 tháng)<br /> - Hdd 500gb ( bảo hành 24 tháng)<br /> - Vga 1060 3g ( bảo hành 06 tháng) <br /> - Vỏ kenoo k300 + 3 fan đa sắc + tản tomato<br /> Giá: 6.500.000<br /> Trả trước: 2.600.000<br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 17<br /> - Main MSI H510M  ( bảo hành 36 tháng)<br /> - Cpu i3 10100f ( bảo hành 36 tháng)<br /> - Ram  8g ddr4 buss 2666  ( bảo hành 36 tháng)<br /> - Nguồn Centaur 450w ( bảo hành 36 tháng)<br /> - Vga 730 2g ddr5  ( bảo hành 36 tháng)<br /> - SSD 120gb ( bảo hành 36 tháng)<br /> - Vỏ văn phòng<br /> Giá: 6.690.000<br /> Trả trước: 2.676.000<br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 18<br /> Main H510m-b ( bảo hành 36 tháng)<br /> Cpu i3 10100f ( bảo hành 36 tháng)<br /> Ram 8g ddr4  ( bảo hành 36 tháng)<br /> nguồn 450w 80 plus ( bảo hành 36 tháng)<br /> VGa 1060 3g ( bảo hành 06 tháng)<br /> SSD nvme 128gb ( bảo hành 36 tháng)<br /> Hdd 500gb ( bảo hành 24 tháng)<br /> Vỏ led + 3 fan<br /> Giá: 7.999.000<br /> trả trước: 3.200.000<br /> ------------------------<br /> &gt;&gt;&gt; Cấu hình 19<br /> - Main H110 ( bảo hành 24 tháng)<br /> - Cpu i5 6400( bảo hành 06 tháng<br /> - Ram 8gb ddr4  ( bảo hành 36 tháng)<br /> - SSD 240g( bảo hành 36 tháng)<br /> - Vga 1050 2g/ 960 2g ( bảo hành 06 tháng)<br /> - Nguồn 450w 80 plus ( bảo hành 06 tháng)<br /> - Vỏ lumix + 3 fan đa sắc<br /> Giá:6.050.000<br /> trả trước 2.420.000<br /> --------------------------<br /> &gt;&gt;&gt; Cấu hình 20<br /> - Main H110 ( bảo hành 24 tháng)<br /> - Cpu i5 6400( bảo hành 06 tháng<br /> - Ram 8gb ddr4  ( bảo hành 36 tháng)<br /> - SSD 240g( bảo hành 36 tháng)<br /> - Vga RX 6500 4g( bảo hành 36 tháng)<br /> - Nguồn 550W 80 plus ( bảo hành 36 tháng)<br /> - Vỏ led + 3 fan đa sắc<br /> Giá:7.899.000<br /> trả trước 3.160.000<br /> <br /> ------------------<br /> &gt;&gt;&gt; Cấu hình 21<br /> - Main Asus/ giga/ MSI H410M  ( bảo hành 36 tháng)<br /> - Cpu i3 10100f tray ( bảo hành 36 tháng)<br /> - Ram 8g ddr4 buss 2666 ( bảo hành 36 tháng)<br /> - Vga 560 4g( bảo hành 36 tháng)<br /> - Nguồn Centaur 450w ( bảo hành 36 tháng)<br /> - SSd 120gb ( bảo hành 36 tháng)<br /> - Vỏ XA20<br /> Giá: 7.899.000<br /> Trả trước chỉ từ: 3.160.000<br /> ------------------<br /> 📍 𝐂𝐚̂́𝐮 𝐡𝐢̀𝐧𝐡 𝐜𝐡𝐨̛𝐢 𝐜𝐚́𝐜 𝐠𝐚𝐦𝐞 𝐡𝐨𝐭 𝐏𝐮𝐛𝐠 𝐏𝐂, 𝐆𝐭𝐚 𝐕, 𝐂𝐬𝐠𝐨, 𝐅𝐢𝐟𝐚, 𝐋𝐨𝐥, 𝐏𝐡𝐨𝐭𝐨𝐬𝐡𝐨𝐩 𝐀𝐢 , 𝐩𝐫𝐢𝐦𝐞𝐫 ......<br /> &gt;&gt;&gt; Cấu hình 22<br /> - Main H81 ( bảo hành 24 tháng)<br /> - Cpu i5 4570 &quot;upto 3.60GHz, 4 nhân 4 luồng&quot;( bảo hành 06 tháng)<br /> - Ram 8g ddr3 ( bảo hành 36 tháng)<br /> - vga RX6500 4g ( bảo hành 36 tháng)<br /> - Nguồn 500w 80 plus ( bảo hành 36 tháng)<br /> - Ssd 240gb ( bảo hành 36 tháng)<br /> - Vỏ XA20<br /> Giá:7.099.000<br /> Trả trước chỉ từ 2.840.000<br /> ----------------------<br /> &gt;&gt;&gt; Cấu hình 23<br /> - Main H81 ( bảo hành 24 tháng)<br /> - Cpu i5 4570 &quot;upto 3.60GHz, 4 nhân 4 luồng&quot;( bảo hành 06 tháng)<br /> - Ram 8g ddr3 ( bảo hành 36 tháng)<br /> - vga 1050 2g/ 960 2g ( bảo hành 06 tháng)<br /> - Nguồn 450w 80 plus ( bảo hành 36 tháng)<br /> - Ssd 240gb ( bảo hành 36 tháng)<br /> - Vỏ led + 3 fan đa sắc<br /> Giá:5.199.000<br /> Trả trước: 2.080.000<br /> ---------------<br /> &gt;&gt;&gt;&gt; Cấu hình 24<br /> -Main h110 ( bảo hành 03 tháng)<br /> - i5 6500 ( bảo hành 03 tháng)<br /> - Ram 8g ddr4 (bảo hành 36 tháng)<br /> - Nguồn 500w  ( bảo hành 6 tháng)<br /> - ssd 240gb ( bảo hành 36 tháng)<br /> - VGA 1060 3g( bảo hành 06 tháng)<br /> - Vỏ XA 20<br /> Giá: 5.690.000<br /> Trả trước 2.279.000<br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 25<br /> - Main H81 ( bảo hành 24 tháng)<br /> - Cpu i5 4570 &quot;upto 3.60GHz, 4 nhân 4 luồng&quot;( bảo hành 06 tháng)<br /> - Ram 8g ddr3 ( bảo hành 36 tháng)<br /> - vga 750ti 4g ( bảo hành 24 tháng)<br /> - Nguồn 450W 80 plus ( bảo hành 36 tháng)<br /> - Ssd 240gb ( bảo hành 36 tháng)<br /> - Vỏ led+ 3 fan đa sắc<br /> Giá:5.399.000<br /> Trả trước: 2.160.000<br /> <br /> -------------------<br />  &gt;&gt;&gt; Cấu hình 26<br /> - Main H81 ( bảo hành 24 tháng)<br /> - Cpu i5 4570 &quot;upto 3.60GHz, 4 nhân 4 luồng&quot;( bảo hành 06 tháng)<br /> - Ram 8g ddr3 ( bảo hành 36 tháng)<br /> - vga 560 4g ( bảo hành 36 tháng)<br /> - Nguồn 550W 80 plus ( bảo hành 36 tháng)<br /> - Ssd 240gb ( bảo hành 36 tháng)<br /> - Vỏ led + 3 fan đa sắc<br /> Giá: 6.399.000<br /> Trả trước: 2.560.000<br /> ---------------------<br /> &gt;&gt;&gt; Cấu hình 27<br />  Main gigabye/ MSI/ asus H410M ( bảo hành 36 tháng)<br /> - Cpu i3 10100f &quot; upto 4.3 GHz 4 Cores 8 Threads&quot; ( bảo hành 36 tháng)<br /> - Vga RX6500 4g ( bảo hành 6 tháng)<br /> - Ram  8g ddr4 ( bảo hành 36 tháng)<br /> - SSD 240gb ( bảo hành 36 tháng)|<br /> - Nguồn 550W 80plus( bảo hành 36 tháng)<br /> - Vỏ led + 3 fan đa sắc<br /> Giá: 9.399.000 <br /> Trả trước:3.760.000<br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 28<br />  Main gigabye/ MSI/ asus H410M ( bảo hành 36 tháng)<br /> - Cpu i3 10100f &quot; upto 4.3 GHz 4 Cores 8 Threads&quot; ( bảo hành 36 tháng)<br /> - Vga galax 3050 8g ( bảo hành 36 tháng)<br /> - Ram  8g ddr4 ( bảo hành 36 tháng)<br /> - SSD 240gb ( bảo hành 36 tháng)<br /> - Nguồn 550W 80 plus ( bảo hành 36 tháng)<br /> - Vỏ led + 3 fan đa sắc<br /> Giá: 11.199.000<br /> Trả trước: 4.480.000<br /> --------------------<br /> &gt;&gt;&gt; Cấu hình 29<br /> - Main Asus/MSI H410M ( bảo hành 36 tháng)<br /> - Cpu i3 10100f ( bảo hành 06 tháng)<br /> - Ram  8g ddr4 Buss 2666 ( bảo hành 36 tháng)<br /> - SSDbr 240gb ( bảo hành 36 tháng)<br /> - Nguồn 450w 80 plus ( bảo hành 36 tháng)<br /> - Vga 1060 3g( bảo hành 06 tháng)<br /> - VỎ led + 3 fan đa sắc <br /> Giá: 7.999.000<br /> Trả trước: 3.200.000<br /> ---------------<br /> &gt;&gt;&gt; Cấu hình 30<br /> - Main MSI H510M( bảo hành 36 tháng)<br /> - CPU i3 10100f ( bảo hành 36 tháng)<br /> - Ram br 8g ddr4 buss 2666 ( bảo hành 36 tháng)<br /> - SSD br nvme 128gb ( bảo hành 36 tháng)<br /> - Hdd 500gb ( bảo hành 24 tháng)<br /> - Vga 560 4g ( bảo hành 36 tháng)<br /> - NGuồn 550W 80 plus ( bảo hành 36 tháng)<br /> - Vỏ led + 3 fan đa sắc<br /> Giá: 8.899.000<br />  Trả trước: 3.560.000<br /> -------------------------<br /> &gt;&gt;&gt; Cấu hình 31<br /> - Main H110( bảo hành 24 tháng)<br /> - CPU i5 6500( bảo hành 06 tháng)<br /> - Ram br 8g ddr4 buss 2666( bảo hành 36 tháng)<br /> - SSD br 240gb ( bảo hành 36 tháng)<br /> - Vga 560 4g ( bảo hành 36 tháng)<br /> - NGuồn 550W 80 plus ( bảo hành 36 tháng)<br /> - Vỏ led + 3 fan đa sắc<br /> Giá: 7.099.000<br />  Trả trước: 2.840.000<br /> ----------------------------<br /> &gt;&gt;&gt; Cấu hình 32<br /> - Main MSI H510m-b ( bảo hành 36 tháng)<br /> - CPU i3 10100f ( bảo hành 36 tháng)<br /> - Ram  8g ddr4 buss 2666 ( bảo hành 36 tháng)<br /> - SSD nvme 128gb ( bảo hành 36 tháng)<br /> - Hdd 500gb ( bảo hành 24 tháng)<br /> - Vga galax 3050 8g ( bảo hành 36 tháng)<br /> - NGuồn Centaur 650w 80 plus( bảo hành 36 tháng)<br /> - Vỏ led + 3 fan đa sắc<br /> - Vỏ 11.699.000<br />  Trả trước: 4.680.000<br /> ------------------------<br /> &gt;&gt;&gt; Cấu hình 33<br /> - Main Asus H510M  ( bảo hành 36 tháng)<br /> - Cpu i5 11400f ( bảo hành 36 tháng)<br /> - Ram br 8g ddr4 ( bảo hành 36 tháng)<br /> - Vga RX6500 4g ( bảo hành 36 tháng)<br /> - Nguồn 550w 80 plus ( bảo hành 36 tháng)<br /> - Ssd br nvme 128g( bảo hành 36 tháng)<br /> - Hdd 500gb ( bảo hành 24 tháng)<br /> - Vỏ led + 3 fan đa sắc<br /> Giá: 10.499.000<br /> Trả trước: 4.199.000<br /> --------------------<br /> &gt;&gt;&gt; Cấu hình 34<br /> - Main Asus H510M  ( bảo hành 36 tháng)<br /> - Cpu i5 11400f ( bảo hành 36 tháng)<br /> - Ram  8g ddr4 ( bảo hành 36 tháng)<br /> - Vga MSI 3060 12g ( bảo hành 36 tháng)<br /> - Nguồn Centaur 750w 80 plus ( bảo hành 36 tháng)<br /> - Ssd br nvme 128g( bảo hành 36 tháng)<br /> - Hdd 500gb ( bảo hành 24 tháng)<br /> - Vỏ led + 3 fan đa sắc<br /> Giá: 14.599.000<br /> Trả trước: 5.840.000<br /> ----------------------<br />  &gt;&gt;&gt; Cấu hình 35<br /> - Main MSI/ Asus H610M  ( bảo hành 36 tháng)<br /> - Cpu i3 12100f ( bảo hành 36 tháng)<br /> - Ram 8g ddr4 ( bảo hành 36 tháng)<br /> - Vga galax 3050 8g ( bảo hành 36 tháng)<br /> - Nguồn Centaur 650w 80 plus ( bảo hành 36 tháng)<br /> - Ssd br nvme 128g( bảo hành 36 tháng)<br /> - Hdd 500gb ( bảo hành 24 tháng)<br /> - Vỏ led + 3 fan đa sắc<br /> Giá: 12.500.000<br /> Trả trước: 5.000.000<br /> <br /> ----------------------<br /> <br /> &gt;&gt;&gt; Cấu hình 36<br /> - Main Asus/MSI/giga H410 (bảo hành 36 tháng)<br /> - Cpu i3 10100f (bảo hành 36 tháng)<br /> - Ram br 8g ddr4 (bảo hành 36 tháng)<br /> - Vga 1650 4g (bảo hành 36 tháng)<br /> - Nguồn Centaur 450W 80 plus (bảo hành 36 tháng)<br /> - Ssd 240gb (bảo hành 36 tháng)<br /> - Vỏ led<br /> Giá: 9.199.000<br /> Trả trước: 3.680.000<br /> --------------------<br /> &gt;&gt;&gt; Cấu hình 37<br /> - Main Asus H510M ( bảo hành 36 tháng)<br /> - Cpu i5 11400f tray ( bảo hành 36 tháng)<br /> - Ram 8g ddr4 ( bảo hành 36 tháng)<br /> - Vga 1060 3g ( bảo hành 06 tháng)<br /> - Nguồn 450w 80 plus ( bảo hành 36 tháng)<br /> - Ssd nvme 128gb ( bảo hành 36 tháng)<br /> - Hdd 500gb ( bảo hành 24 tháng)<br /> - Vỏ led + 3 fan đa sắc<br /> Giá: 8.599.000<br /> Trả trước: 3.350.000<br /> --------------------<br /> &gt;&gt;&gt; Cấu hình 38<br /> - Main Asus/MSI/giga H410 ( bảo hành 36 tháng)<br /> - Cpu i3 10100f ( bảo hành 36 tháng)<br /> - Ram 16g ddr4 ( bảo hành 36 tháng)<br /> - Vga galax 1650 4g ( bảo hành 36 tháng)<br /> - Nguồn Centaur 550w ( bảo hành 36 tháng)<br /> - Ssd 240gb ( bảo hành 36 tháng)<br /> - Vỏ Kenoo MK500 + 3 fan đa sắc<br /> Giá: 9.799.000<br /> Trả trước: 4.000.000<br /> --------------------<br /> &gt;&gt;&gt;&gt; Cấu hình 39<br /> - Main  MSi/ Asus H610M ( bảo hành 36 tháng)<br /> -cpu i3 12100F ( bảo hành 36 tháng)<br /> - Ram 8g ddr4 buss 2666 ( bảo hành 36 tháng)<br /> - SSD 240gb ( bảo hành 36 tháng)<br /> - vga galax 1650 4g ( bảo hành 36 tháng)<br /> - Nguồn Centaur 450w 80 plus ( bảo hành 36 tháng)<br /> - Vỏ led + 4 fan đỏ/ 3 fan đa sắc<br /> Giá: 10.099.000<br /> trả trước: 4.040.000<br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 40<br /> - Main MSI B560M  ( bảo hành 36 tháng)<br /> - Cpu i3 10100f ( bảo hành 36 tháng)<br /> - Ram 16gb ddr4 buss 2666  ( bảo hành 36 tháng)<br /> - Vga galax 1650 4g ( bảo hành 36 tháng)<br /> - Nguồn 550w ( bảo hành 36 tháng)<br /> - SSD NVme 512gb ( bảo hành 36 tháng)<br /> - Vỏ led + 4 fan đỏ / 3 fan đa sắc<br /> Giá: 10.500.000<br /> Trả trước: 4.200.000<br /> -------------------<br /> &gt;&gt;&gt;Cấu hình 41<br /> - Main MSI/ Asus H610   ( bảo hành 36 tháng)<br /> - Cpu i3 12100f tray ( bảo hành 36 tháng)<br /> - Ram 16gb ddr4 buss 2666  ( bảo hành 36 tháng)<br /> - Vga  galax 3050 8g ( bảo hành 36 tháng)<br /> - Nguồn Centaur 550w 80 plus ( bảo hành 36 tháng)<br /> - SSD BR NVme 256  ( bảo hành 36 tháng)<br /> - Vỏ k300 + 3 fan đa sắc + tản tomato<br /> Giá: 12.599.000<br /> Trả trước: 5.040.000<br /> -----------------------<br /> 📍 𝐑𝐞𝐧𝐝𝐞𝐫, Đ𝐨̂̀ 𝐇𝐨̣𝐚 𝐂𝐚𝐨 , 𝐂𝐡𝐚̣𝐲 𝐠𝐢𝐚̉ 𝐥𝐚̣̂𝐩 𝐍𝐨𝐱 𝐠𝐚𝐦𝐞 𝐡𝐨𝐭 𝐏𝐮𝐛𝐠 𝐏𝐂, 𝐆𝐭𝐚 𝐕, 𝐂𝐬𝐠𝐨, 𝐅𝐢𝐟𝐚, 𝐋𝐨𝐥, 𝐏𝐡𝐨𝐭𝐨𝐬𝐡𝐨𝐩 𝐀𝐢 , 𝐩𝐫𝐢𝐦𝐞𝐫 ......<br /> &gt;&gt;&gt; Cấu hình 42 chạy 5-10 acc<br /> - Main X99 ( bảo hành 06 tháng)<br /> - Cpu E5 2680 v4 ( bảo hành 06 tháng)<br /> - Ram 32gb 16*2gb ddr4 ( bảo hành 06 tháng)<br /> - SSD  nvme 256gb  ( bảo hành 36 tháng)<br /> - Nguồn xigamtek x550 80 plus ( bảo hành 36 tháng)<br /> - VGA 1070 8g ( bảo hành 06 tháng)<br /> - Tản tomato ( bảo hành 03 tháng)<br /> - Vỏ Xigmatek XA20<br /> Giá: 8.399.000<br /> trả trước : 3.360.000<br /> -------------<br /> &gt;&gt;&gt; Cấu hình 43<br /> - Main MSI B560M ( bảo hành 36 tháng)<br /> - Cpu i5 11400f tray ( bảo hành 36 tháng)<br /> - Ram 8g ddr4 ( bảo hành 36 tháng)<br /> - Vga RX6600 8g ( bảo hành 36 tháng)<br /> - Nguồn 550w 80 plus ( bảo hành 36 tháng)<br /> - SSd br 128gb nvme( bảo hành 36 tháng)<br /> - HDD 500gb ( bảo hành 24 tháng)<br /> - Vỏ led + 3 fan đa sắc<br /> Giá: 12.199.000<br /> Trả trước: 4.880.000<br /> ------------------<br /> &gt;&gt;&gt; Cấu hình 44<br /> - Main MSI B560M  ( bảo hành 36 tháng)<br /> - Cpu i5 11400f tray ( bảo hành 36 tháng)<br /> - Ram  8g ddr4 ( bảo hành 36 tháng)<br /> - Vga galax 3050 8g ( bảo hành 36 tháng)<br /> - Nguồn aigo 650W  ( bảo hành 36 tháng)<br /> - SSd  nvme 128g ( bảo hành 36 tháng)<br /> - Hdd 500gb ( bảo hành 24 tháng)<br /> - Vỏ led + 4 fan led đỏ/ 3 fan đa sắc + tản Sama k400d<br /> Giá: 12.999.000<br /> Trả trước: 5.200.000<br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 45<br /> - Main Asus H610M ( bảo hành 36 tháng)<br /> - Cpu i5 12400f tray( bảo hành 36 tháng)<br /> - Ram  8g ddr4 ( bảo hành 36 tháng)<br /> - Vga RX6600 4gb ( bảo hành 36 tháng)<br /> - Nguồn CT650w ( bảo hành 36 tháng)<br /> - SSd br nvme 128gb ( bảo hành 36 tháng)<br /> - Hdd 500gb ( bảo hành 24 tháng)<br /> - Vỏ led + 3 fan đa sắc<br /> Giá: 13.099.000<br /> Trả trước: 5.240.000<br /> ----------------<br /> &gt;&gt;&gt; Cấu hình 46<br /> - Main gigabye B760M D5  ( bảo hành 36 tháng)<br /> - Cpu i5 12400f tray ( bảo hành 36 tháng)<br /> - Ram Gskill 16gb d5 buss 5600 ( bảo hành 36 tháng)<br /> - Vga galax 1650 4g ( bảo hành 36 tháng)<br /> - Nguồn 550w 80 plus ( bảo hành 36 tháng)<br /> - SSd br nvme 128gb ( bảo hành 36 tháng)<br /> - Hdd 500gb ( bảo hành 24 tháng)<br /> - Vỏ led+ 3 fan đa sắc + Tản Centaur CT-AIR03 <br /> Giá: 14.199.000<br /> Trả trước: 5.680.000<br /> ----------------<br /> &gt;&gt;&gt; Cấu hình 47<br /> - Main giga/ MSI/ Asus B560M 4 khe ram ( bảo hành 36 tháng)<br /> - Cpu i5 11400f tray ( bảo hành 36 tháng)<br /> - Ram  8g ddr4 ( bảo hành 36 tháng)<br /> - Vga galax 3050 8g ( bảo hành 36 tháng)<br /> - Nguồn Centaur 650w ( bảo hành 36 tháng)<br /> - SSd  256gb nvme ( bảo hành 36 tháng)<br /> - Vỏ led + 4 fan led đỏ + Tản Centaur CT-AIR03 <br /> Giá: 13.599.000<br /> Trả trước: 5.440.000<br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 48<br /> - Main MSI H610M ( bảo hành 36 tháng)<br /> - Cpu i5 12400f tray ( bảo hành 36 tháng)<br /> - Ram  8g ddr4 ( bảo hành 36 tháng)<br /> - Vga galax 3050 8g ( bảo hành 36 tháng)<br /> - Nguồn 550w 80 plus( bảo hành 36 tháng)<br /> - SSd 240gb ( bảo hành 36 tháng)<br /> - Vỏ light đen/ trắng + 3 fan đa sắc+ tản khí Centaur<br /> Giá: 13.299.000<br /> Trả trước : 5.320.000<br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 49<br /> - Main Asus H610M ( bảo hành 36 tháng)<br /> - Cpu i5 12400f tray ( bảo hành 36 tháng)<br /> - Ram  8g ddr4 ( bảo hành 36 tháng)<br /> - Vga MSI 3060 12g ( bảo hành 36 tháng)<br /> - Nguồn Centaur 750w 80 plus ( bảo hành 36 tháng)<br /> - SSd  256gb nvme ( bảo hành 36 tháng)<br /> - Vỏ snow đen/ trắng + 1 fan đa sắc + Tản centaur<br /> Giá: 16.199.000<br /> Trả trước: 6.480.000<br /> <br /> --------------------<br /> &gt;&gt;&gt;&gt; Cấu hình 50<br /> - Main MSI B760M ( bảo hành 36 tháng)<br /> - Cpu i5 12400f tray ( bảo hành 36 tháng)<br /> - Ram  8g ddr4  ( bảo hành 36 tháng)<br /> - SSD  NVME 250gb  ( bảo hành 36 tháng)<br /> - Nguồn Xigmatek T750 ( bảo hành 36 tháng)<br /> - Vga MSI gaming X 4060ti 8g ( bảo hành 36 tháng)<br /> -  Vỏ V309  + 3 fan đa sắc + tản Centaur<br /> Giá: 21.799.000<br /> Trả trước: 10.899.000<br /> -------------------<br /> &gt;&gt;&gt;  Cấu hình 51 Chuyên render, đồ hoạ 2d 3d max, gaming<br /> - Main Asrock B450M  ( bảo hành 36 tháng)<br /> - Cpu ryzen 7 2700 ( bảo hành 36 tháng)<br /> - Ram br 16g ddr4 buss 2666 8*2 ( bảo hành 36 tháng)<br /> - Vga galax 1650 4g( bảo hành 36 tháng)<br /> - Nguồn Centaur 450w  ( bảo hành 36 tháng)<br /> - SSd br 240gb ( bảo hành 36 tháng)<br /> - Vỏ led + 3 fan đa sắc <br /> Giá: 12.599.000<br /> Trả trước: 5.040.000<br /> ------------------- <br /> &gt;&gt;&gt;&gt; Cấu hình 52<br /> - Main gigabyte/ MSI B560M  ( bảo hành 36 tháng)<br /> - CPu i5 11400f tray ( bảo hành 36 tháng)<br /> - Ram  8g ddr4 buss 2666 ( bảo hành 36 tháng)<br /> - ssd  nvme 256gb  ( bảo hành 36 tháng)<br /> - Nguồn 550w 80 plus ( bảo hành 36 tháng)<br /> - Vga galax 3050 8g ( bảo hành 36 tháng)<br /> -Vỏ kenoo k300+ 3 fan đa sắc<br /> Giá: 12.599.000<br /> Trả trước: 5.040.000<br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 53<br /> - Main Gigabyte B560M DS3H( bảo hành 36 tháng)<br /> - Cpu i5 11400f tray ( bảo hành 36 tháng)<br /> - Ram  16g  ddr4 buss 2666 ( bảo hành 36 tháng)<br /> - Vga MSI 3060 12gb ( bảo hành 36 tháng)<br /> - Nguồn Centaur 750W 80plus ( bảo hành 36 tháng)<br /> - SSd  nvme 250gb ( bảo hành 36 tháng)<br /> -Hdd 500gb ( bảo hành 24 tháng)<br /> - Vỏ kenoo K300 + cr1000<br /> Giá: 16.599.000<br /> Trả trước: 6.640.000<br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 54<br /> - Main X99 F8d ( bảo hành 06 tháng)<br /> - Cpu E5 2680 V4 *2 ( bảo hành 06 tháng)<br /> - Ram 32gb *4 ddr4 ( bảo hành 06 tháng)<br /> - Vga 1070 8g ( bảo hành 06 tháng)<br /> - Nguồn Xigmatek X650 80plus ( bảo hành 36 tháng)<br /> - SSd  nvme 256 ( bảo hành 36 tháng)<br /> - tản khí tomato *2<br /> - Vỏ Kenoo ea600 + 3 fan<br /> Giá: 15.399.000<br /> trả trước: 6.160.000<br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 55<br /> - Main MSI B760M ( bảo hành 36 tháng)<br /> - Cpu i5 12400f ( bảo hành 36 tháng)<br /> - Ram br 16g ddr4 buss 2666 ( bảo hành 36 tháng)<br /> - Vga galax 3050 8g ( bảo hành 36 tháng)<br /> - Nguồn Centaur 650w 80 plus ( bảo hành 36 tháng)<br /> - SSd 512gb NVME ( bảo hành 36 tháng)<br /> - Vỏ kenoo K300+ tản khí<br /> Giá: 15.399.000<br /> trả trước: 6.160.000<br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 56<br /> - Main Gigabyte/Asus B760M gaming ( bảo hành 36 tháng)<br /> - Cpu i5 13400f ( bảo hành 36 tháng)<br /> - Ram br 16g ddr4 buss 2666 ( bảo hành 36 tháng)<br /> - Vga galax 3050 8g ( bảo hành 36 tháng)<br /> - Nguồn Centaur 650w ( bảo hành 36 tháng)<br /> - SSd 256gb NVME ( bảo hành 36 tháng)<br /> - Hdd 500gb (Bảo hành 24 tháng)<br /> - Vỏ led  + 3 fan đa sắc + Tản Centaur CT-AIR03 <br /> Giá: 17.599.000<br /> trả trước: 7.040.000<br /> -------------------<br /> &gt;&gt;&gt; Cấu hình 57<br /> - Main X99 F8d ( bảo hành 12 tháng)<br /> - Cpu E5 2673  V3 * 2 ( bảo hành 12 tháng)<br /> - Ram 64gb ddr3 ( bảo hành 12 tháng)<br /> - Vga  rx6500 4g ( bảo hành 36 tháng)<br /> - Nguồn Xigamtek X650 ( bảo hành 36 tháng)<br /> - SSd  nvme 256 ( bảo hành 36 tháng)<br /> - tản tomato *2<br /> - Vỏ kenoo ea600  <br /> Giá: 12.599.000<br /> trả trước : 5.040.000<br /> -----------------<br /> &gt;&gt;&gt;&gt; Cấu hình 58<br /> - Main X99 duor cpu( bảo hành 12 tháng)<br /> - Cpu E5 2680 V4 *2 ( bảo hành 12 tháng)<br /> - Ram 128gb ddr4 ( bảo hành 12 tháng)<br /> - Vga  1650 4g  ( bảo hành 36 tháng)<br /> - Nguồn Centaur 450w 80 plus ( bảo hành 36 tháng)<br /> - SSd Kingmax nvme 256 ( bảo hành 36 tháng)<br /> - tản Cr1000<br /> - Vỏ Sama 3301 + 3 fan led RGB<br /> Giá: liên hệ<br /> ---------------------<br /> &gt;&gt;&gt;&gt; Cấu hình 59<br /> Main gigabyte B760M DDR5( bảo hành 36 tháng)<br /> Cpu i5 12400f ( bảo hành 36 tháng)<br /> Ram gskill 16gb d5 buss 5600 ( bảo hành 36 tháng)<br /> SSD adata NVMe 500g ( bảo hành 36 tháng)<br /> HDD 1T ( bảo hành 24 tháng)<br /> Nguồn Centaur 650w 80 plus ( bảo hành 36 tháng)<br /> Vga galax 3050 8g ( bảo hành 36 tháng)<br /> Vỏ Odyssey đen + 4 fan RGB lục giác + khiển hub<br /> Tản Sama đen<br /> Giá: 18.399.000<br /> Trả trước: 7.360.000<br /> ------------------------<br /> &gt;&gt;&gt; Cấu hình 60<br /> - Main Giga aorus Z690M ( bảo hành 36 tháng)<br /> - Cpu i5 13600k ( bảo hành 36 tháng)<br /> - Ram Adata D50 8g *2 buss 3200 RGB ( bảo hành 36 tháng)<br /> - VGa galax 3050 8g ( bảo hành 36 tháng)<br /> - Nguồn Centaur 650w 80 plus ( bảo hành 36 tháng)<br /> - Ổ cứng apacer NVME 512gb ( bảo hành 36 tháng)<br /> - HDD WD 1T (bảo hành 24 tháng)<br /> -  Vỏ Kenoo Luxe V1 trắng + tản nước 360 coolmoon+ 7 fan đa rgb <br /> Giá:24.399.000<br /> trả trước: 12.200.000 <br /> --------------------<br /> &gt;&gt;&gt; Cấu hình 61<br /> - Main Giga Z690M ( bảo hành 36 tháng)<br /> - Cpu i5 12600K ( bảo hành 36 tháng)<br /> - Ram D35G 16g ddr4 buss 3200 ( bảo hành 36 tháng)<br /> - SSD kingston nvme  1T ( bảo hành 36 tháng)<br /> - VGa Asus 3060 12gb ( bảo hành 36 tháng)<br /> - Nguồn Centaur 750w ( bảo hành 36 tháng<br /> - Vỏ kenoo EA600  + tản CPu<br /> Giá:  22.399.000<br /> Trả trước: 11.200.000<br /> ------------------- <br /> &gt;&gt;&gt; Cấu hình 62<br /> - Main Gigabyte/ Asus Z790 ( bảo hành 36 tháng)<br /> - Cpu i9 12900k ( bảo hành 36 tháng)<br /> - Ram D35g 16gb ddr4 buss 3200 rgb ( bảo hành 36 tháng)<br /> - SSd  nvme 512gb ( bảo hành 36 tháng)<br /> - Hdd seagate 1t ( bảo hành 24 tháng)<br /> - Vga MSI 3060 12gb  ( bảo hành 36 tháng)<br /> - Nguồn Centaur 750w ( bảo hành 36 tháng)<br /> - Vỏ EA600 + 3 fan <br /> - Tản Cpu tomato<br /> Giá: 28.399.000<br /> Trả trước: 14.200.000<br /> <br /> ----------------------<br /> &gt;&gt;&gt; Cấu hình 63<br /> - Main gigabyte Z690M (bảo hành 36 tháng)<br /> - Cpu i7 12700k ( bảo hành 36 tháng)<br /> - Ram D35G 16gb ddr4 buss 3200 ( bảo hành 36 tháng)<br /> - Vga MSI RTX4070 Ventus 2X 12G OC  ( bảo hành 36 tháng)<br /> - SSd BR nvme 256gb ( bảo hành 36 tháng)<br /> - Hdd seagate 1T( bảo hành 24 tháng)<br /> - Nguồn Coolermaster 750W ( bảo hành 36 tháng)<br /> - Vỏ EA600 + 4 fan led rgb + hub khiển<br /> - Tản cpu Hyper<br /> Giá: 34.299.000<br /> Trả trước: 17.150.000<br /> ----------------------<br /> &gt;&gt;&gt; Cấu hình 64<br /> - Main Gigabyte/ Asus Z790 (Bảo hành 36 tháng)<br /> - CPU INTEL CORE i7-13700K (UP TO 5.40GHZ, 16 NHAN 24 LUONG, 25M CACHE.RAPTOR LAKE<br /> - Ram Gskill 32G (16Gbx 2)DDR4 3600 MHz ( bảo hành 36 tháng)<br /> - SSD  NVME 1T ( bảo hành 36 tháng)<br /> - VGA RIX 3060 12gb ( bảo hành 36 tháng)<br /> - NGUON COOLER MASTER 750W 80 PLUS  ( bảo hành 36 tháng)<br /> - Vỏ EA600 + 3 fan + tản hyper xigmatek<br /> Giá: 31.890.000<br /> Trả trước: 15.945.000<br /> ----------------------<br /> &gt;&gt;&gt; Cấu hình 65<br /> - Main gigabyte/ Asus Z790 (bảo hành 36 tháng)<br /> - Cpu i9 13900k ( bảo hành 36 tháng)<br /> - Ram D35G 32gb &quot;16gb *2&quot; ddr4 buss 3200 ( bảo hành 36 tháng)<br /> - Vga 3060 12gb( bảo hành 36 tháng)<br /> - SSd  nvme 512gb ( bảo hành 36 tháng)<br /> - Hdd seagate 1T ( bảo hành 24 tháng)<br /> - Nguồn Coolermaster 750W ( bảo hành 36 tháng)<br /> - Vỏ EA600 + 4 fan led rgb + hub khiển<br /> - Tản cpu  killer<br /> Giá: 36.999.000<br /> trả trước: 18.500.000<br /> ----------------------------------<br /> &gt;&gt;&gt; Cấu hình 66<br /> - Main gigabyte/ Asus Z790 (bảo hành 36 tháng)<br /> - Cpu i9 14900K( bảo hành 36 tháng)<br /> - Ram D35G 32gb &quot;16gb *2&quot; ddr4 buss 3200 ( bảo hành 36 tháng)<br /> - Vga 4070 12gb( bảo hành 36 tháng)<br /> - SSd Br nvme 512gb ( bảo hành 36 tháng)<br /> - Hdd seagate 1T ( bảo hành 24 tháng)<br /> - Nguồn Coolermaster 750W ( bảo hành 36 tháng)<br /> - Vỏ Odyssey + 4 fan led rgb + hub khiển<br /> - Tản cpu  killer<br /> Giá: liên hệ<br /> -------------------------------------<br /> Ư𝐔 𝐃Ã𝐈 𝐊𝐇Ủ𝐍𝐆 𝐊𝐇𝐈 𝐌𝐔𝐀 𝐇À𝐍𝐆 𝐓Ạ𝐈 𝐇Ả𝐈 𝐏𝐇Ò𝐍𝐆 𝐂𝐎𝐌𝐏𝐔𝐓𝐄𝐑<br /> ✅ Miễn phí vệ sinh và bảo dưỡng máy tính trọn đời máy<br /> ✅Miễn phí bảo hành phần cứng tại nhà<br /> ✅Miễn phí đổi máy trong 1 tuần đầu nếu dùng máy không ưng ý hoặc muốn đổi lên cấu hình cao hơn.<br /> ✅Ngập tràn quà tặng đi kèm khi mua PC hoặc Laptop tại Hải Phòng Computer<br /> ✅Tất cả linh kiện máy tính đều nhập chính hãng, bảo hành lên đến 36 tháng.<br /> 👉HỖ TRỢ TRẢ GÓP:<br /> <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fhaiphongcomputer.vn%2Fhuong-dan-mua-tra-gop%2F%3Ffbclid%3DIwAR3IfezCjeDizYmr5poFzyej4oOYUC9Uaj058i_UiOjEVo-9t_rQ-eZR4F0&amp;h=AT01KH_2_u4BZYz7kQg3NMTOsDiN22ctnxvI-pBoUCjAc_bP8N_6kzYaXSjmNW8JsfO8u1rX_IVQ9e8B67ZIe67hdXdSX8tgykfCtFtF4dqMO7LYvSTjlqcLdVse4Wl8gc_puNtdDw\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://haiphongcomputer.vn/huong-dan-mua-tra-gop/</a><br /> 👉CHÍNH SÁCH BẢO HÀNH:<br /> <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fhaiphongcomputer.vn%2Fchinh-sach-bao-hanh-san-pham...%2F%3Ffbclid%3DIwAR3llA0VI4aglW2sNoPbyyRpovvgFkdXH3abzvn65BPZlvmprOF4KAtf4H0&amp;h=AT3cbGqzxzHhH7GBhnw_Q54tDXwz1oouNN65wcZixPtSV751G8h87hOF9u3QZ3iyDm6PEiZQRBRQh2jRUTBu3BmrxLBs2ncQ4CafrJLP30F9tnF-24ckRjX_vHpy5Q1rAICiZj9SDg\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://haiphongcomputer.vn/chinh-sach-bao-hanh-san-pham.../</a><br /> 👉CHÍNH SÁCH VẬN CHUYỂN:<br /> <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fhaiphongcomputer.vn%2Fchinh-sach-van-chuyen%2F%3Ffbclid%3DIwAR2XBRMGBHgPWjWJCGqiOIi5k7AW8314lHLqRsIRhoKVlWM4jSombPRgZW0&amp;h=AT2gA-c4XmzWbg-c6Oml3A9sxHqdCuMRywqB4d_bJf_C5XrIqPeCm6A1mGBg3EHrvGtPcvzQvaDlzkVLE8zUrNxYwbN0K6f5rnJThKfv9QiciehjQpiHZlTshGLe9x2V16tb7O1xdg\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://haiphongcomputer.vn/chinh-sach-van-chuyen/</a><br /> ====================<br /> Hải Phòng Computer chuyên PC Văn Phòng - PC ĐỒ HOẠ- Máy Xeon - PC Game Giá Rẻ - PC Tản Nhiệt Nước - PC AMD -Laptop<br /> ---------------------------------<br /> • Địa chỉ: 82,84 Quán Nam - Lê Chân - Hải Phòng<br /> • Hotline: 0899.256.166<br /> • Website: <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fhaiphongcomputer.vn%2F%3Ffbclid%3DIwAR0-Eq1GWLq55UsVrmIM_M6Gd4WEupymlA7igcl1kr6uJ3r06nVOTzeGglA&amp;h=AT0zH9WBDnkalYXSsu5WjYfI6B393gBTwWsDPIZUjlJUig_Rm5vcy0iSrTvNGpQhtuOdnJ7usCNMOIP7IS3IlPKwlZMRtbGJfYn-5S3yCfBqVSJofRRYQyE3y7zPrpPK-ASAsJ_2cQ\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://haiphongcomputer.vn/</a><br /> • Tiktok: <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fwww.tiktok.com%2F%40haiphongcomputer.vn%3Ffbclid%3DIwAR0F2GVNurCfy3lHwBt2bemEauzc7mh4eYATocDUmiv3DKznLOcC-qCsf2Q&amp;h=AT0Qi80ul-7q6waDAGsC0udRIREf2320GgE4thyZaqep2bVvmc9WhlZUBTGvJNWggX5MDaQT26HsvNcW_yQDvaKkvV6mfWViBNfIdUD0sE_xoXECQuoREerr5TPK9KNdNuvjTikSwQ\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://www.tiktok.com/&#064;haiphongcomputer.vn</a>"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Trung Tâm Laptop Hải Phòng",
                            "disclaimer_label": null,
                            "page_like_count": 5502,
                            "page_profile_uri": "https://facebook.com/100091314824136",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1711954800,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "949047876947999",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 3268435276794623,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "107189848084236",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Trung Tâm Laptop Hải Phòng",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120208191980650345",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": null,
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Vị trí của bạn ở đâu?\"},{\"title\":\"Bạn có thể kiểm tra giá sản phẩm được không?\"},{\"title\":\"Tôi có thể mua hàng không?\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting\":false}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting\":false}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting\":false}},\"user_edit\":false,\"surface\":\"visual_editor_new\",\"ai_generated_welcome_message_impression\":false,\"has_ai_generated_welcome_message\":false}",
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t42.1790-2/10000000_1137749267504846_3351351665494262640_n.?_nc_cat=100&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeF-50l4YomG73o6800jstGu5S0jf18rY-HlLSN_Xytj4QBEsOYVmPIJw7CmpMvr81nWq3C0Y2ZPc75H2zcggj5I&_nc_ohc=LNW3Sfah25kAb7t5DOi&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfDQuZnTTKoYdonFX9kcyLO7LHziJwtJu_jJBYQzBYklMg&oe=6622B360",
                                    "video_sd_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t42.1790-2/436354353_853149456851908_5058382897891345728_n.mp4?_nc_cat=106&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEYqMkW-YRoLPZl7DFS1I-XLspnIZsQCvIuymchmxAK8naij4dxqTrH75XTl2ARvl4i12OLGjBiaoqCOk-HZISL&_nc_ohc=nCI02Qyp5ewAb4XsDD1&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfDJCK6mVXNu1-b9DZC-fGP78VSNGPvYIYebKpnlAFA4WA&oe=6622A8B8",
                                    "watermarked_video_sd_url": "",
                                    "watermarked_video_hd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/436153340_7506216089435248_7939799415241054194_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFmbaGVo1qPuyVKSxYF2k7bqW2RgVwvMNipbZGBXC8w2G3NG6V_3WRdyTOIp1IsarICS16QgY3e4rhXHtFNFyMY&_nc_ohc=Qs5EqTsUaVwAb7OutGq&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfDVIPorkP4D8D-bCp3xIlwMZho6ricuU06xrDyhtFsRNQ&oe=6622D632"
                                }
                            ],
                            "creation_time": 1712598854,
                            "page_id": 107189848084236,
                            "page_name": "Trung Tâm Laptop Hải Phòng",
                            "page_profile_picture_url": "https://scontent.fsgn2-5.fna.fbcdn.net/v/t39.35426-6/436380859_433008315874598_8591215938990285727_n.jpg?stp=dst-jpg_s60x60&_nc_cat=104&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHBfeMiiRvBJBnTrRjV8-TOOHuMOCK6Bqc4e4w4IroGp7SWI5UpkNsut5bPeSieFPE8WQ_7Opeg5sWQV3bW_0Dp&_nc_ohc=9O9uWW46dCAAb7SYX6q&_nc_ht=scontent.fsgn2-5.fna&oh=00_AfBKEf6AkZdQ9zLheQyHFl5_6zPjzBvzjbOy922zi9MFYA&oe=6622D76E",
                            "page_categories": {
                                "200600219953504": "Shopping"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Trung Tâm Laptop Hải Phòng",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/436816331_331179696653137_3722920925994487646_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeExYJN-eryhiuU8wBKS0-2jQI63cd8LlrlAjrdx3wuWuVs73-koBbrSYWdvvwjX2IcZj8vN8LtlsUoU1-_7lsKr&_nc_ohc=1lUQVwL2GbAAb7smGuq&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfDhiqw8uD_fnUdwb48etlYkZxjT9M1g_Rj5tFGGJr4AJA&oe=6622B6B4",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "✅LAPTOP HP SPECTRE 13 – AP0093TU ( i7 - 8th / 16G / 1T SSD ) cảm ứng 2 in 1 đáng mua nhất thời điểm hiện tại #hpsprctre #hpcamung  #HPC"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Trung Tâm Laptop Hải Phòng",
                            "disclaimer_label": null,
                            "page_like_count": 5502,
                            "page_profile_uri": "https://facebook.com/100091314824136",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712905200,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "956121796098606",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 725665582570286,
                        "currency": "",
                        "endDate": 1713078000,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "107189848084236",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Trung Tâm Laptop Hải Phòng",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120204223106600345",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": "Laptop chỉ từ 6Trx dùng bền từ 5 - 7 năm",
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Tư vấn HP 840 g5\",\"response\":\"✅ LAPTOP HP ELITEBOOK 840 G5\\nCPU: i5-8350U\\nRAM: 8 GB\\nỔ CỨNG: SSD 256G\\nĐỒ HOẠ: Intel HD Graphics 620\\nMàn 14' FHD\\n6,590,000đ\\n- Đáp ứng nhu cầu : Văn phòng , đồ hoạ 2D , chơi Liên Minh , CF ....\"},{\"title\":\"Tư vấn Dell 7490\",\"response\":\"✅ LAPTOP DELL LATITUDE 7490\\nCPU: I5 - 8350U\\nRAM: 8GB\\nỔ CỨNG : SSD 256GB\\nĐỒ HOẠ: INTEL GRAPHICS 620\\nMàn : 14' FHD\\n6,490,000đ\\n- Đáp ứng nhu cầu : Văn phòng , đồ hoạ 2D , chơi Liên Minh , CF ....\"},{\"title\":\"Tư vấn dell 5300 i7\",\"response\":\"LAPTOP DELL LATITUDE 5300 CẢM ỨNG\\nCPU: I7- 8665U\\nRAM: 16GB\\nỔ CỨNG : SSD 512G\\nĐỒ HOẠ : Intel HD Graphics\\nMàn : 13' FHD \\n7,990,000đ\\n- Đáp ứng nhu cầu : Văn phòng , đồ hoạ 2D , chơi Liên Minh , CF ....\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Hãy cho biết chúng tôi có thể giúp gì cho bạn.\"}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Hãy cho biết chúng tôi có thể giúp gì cho bạn.\"}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Hãy cho biết chúng tôi có thể giúp gì cho bạn.\"}},\"user_edit\":true,\"surface\":\"visual_editor_new\",\"ice_breakers_edited\":true,\"template_id\":\"1553978818752661\"}",
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t42.1790-2/10000000_1016504679420200_4623961021861105566_n.?_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeES69f1hQNVda4q4lNJ2-lxfv-aqRtkVZB-_5qpG2RVkDmmFJ8xcsFz9Q0ZZB_9TTWV3vy52U7iHTF69tRtRBF4&_nc_ohc=pp3pW7YE8TYAb58aDZD&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfDVee3XbdDtim4sjzKuyiZuVuSRT61Ju0VqtQbCBX0KXA&oe=6622DA40",
                                    "video_sd_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t42.1790-2/414981604_399021382465381_8194027331215341585_n.mp4?_nc_cat=103&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHX9mq0YJgue946N6iIqutVL4N1lLlNSrEvg3WUuU1Ksb1ir5Yu0QAilJgMbl6VwyzhnO8T8N72hIA4fm-j6MZU&_nc_ohc=BK-RP7OHh_AAb5N2h8k&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfAV7T7WoBGScwgwSPGIQbKa1pncwH26eFAMoY8EpT3m_Q&oe=6622CFAB",
                                    "watermarked_video_sd_url": "",
                                    "watermarked_video_hd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/415181551_1487500238461114_9058120897341746905_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFidXtzxb-48wAYghJZpTixDqzWHedC9G8OrNYd50L0b_i1TOSBRQNZVMcD6_LGVF8X2CsmMSqttnwUqVL2oVe0&_nc_ohc=5bSu3dxKYnoAb7L0NB2&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfA0hoqzkQkQ5TJdaNW67irlv1idgN5xWusxvLaRZPK44w&oe=6622C5D6"
                                }
                            ],
                            "creation_time": 1704162959,
                            "page_id": 107189848084236,
                            "page_name": "Trung Tâm Laptop Hải Phòng",
                            "page_profile_picture_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.35426-6/415987742_1105358947452410_436857473582669509_n.jpg?stp=dst-jpg_s60x60&_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEI48uEGhdvSfay-3PMsC66cX-0ydE3u4txf7TJ0Te7ix2qv3BdB399bpbyit5s5VdojKjtHfLi-trHrfOHqjha&_nc_ohc=YUdNyIoj9CUAb5LlGV9&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDfUnouoaHukA9V7UbZbMb8_4javYPSKOmOEx9YtRpYyg&oe=6622AA55",
                            "page_categories": {
                                "200600219953504": "Shopping"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Trung Tâm Laptop Hải Phòng",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/415148474_903276981388920_5194406082889998903_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeH0nPqpn6NQJGZlQqNe-1db_kce_NAYgbj-Rx780BiBuOJ-13vQbqnX43GUpaKeOlugiu2GX4KyzEv3IVaqX_2F&_nc_ohc=WjZlNdEOafkAb599cwR&_nc_oc=Adh26xoPPaUiG9PWB4UAaiSTQiNLo_cIQLTE_-161RhOoellDx0GdZrC11Qd6iD8lNE&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfCvsiLGCp2BvQKZZXAtbpb2APOaHBAAuJXOO33SybCXDg&oe=6622CE97",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "✅𝑪𝒉𝒊̉ 𝒕𝒖̛̀ 6𝑻𝒓𝒙 𝒔𝒐̛̉ 𝒉𝒖̛̃𝒖 𝒏𝒈𝒂𝒚 𝑳𝒂𝒑𝒕𝒐𝒑 𝑴𝒐̉𝒏𝒈 𝒏𝒉𝒆̣ 𝒅𝒖̀𝒏𝒈 5 - 7 𝒏𝒂̆𝒎 𝒗𝒂̂̃𝒏 𝒃𝒆̂̀𝒏 🤩<br /> 👉 𝐇𝐏 𝟖𝟒𝟎 𝐆𝟓 : i5 - 8350U / 8G Ram / 256 SSD / 14&#039; FHD chống loá -- #6trxxx<br /> 👉 𝐃𝐄𝐋𝐋 𝟕𝟒𝟗𝟎 :  i5 - 8350U / 8G Ram / 256 SSD / 14&#039; FHD chống loá - #6trxxx <br /> 👉 𝐃𝐄𝐥𝐥 𝐋𝐚𝐭𝐢𝐭𝐮𝐝𝐞 𝟓𝟑𝟎𝟎 : i7 - 8650U / 16G / 512 SSD / 13&#039; FHD IPS - #7trxxx <br /> 🔹Đ𝐚́𝐩 𝐮̛́𝐧𝐠 𝐭𝐨̂́𝐭 𝐜𝐚́𝐜 𝐧𝐡𝐮 𝐜𝐚̂̀𝐮 : 𝐀𝐮𝐭𝐨 𝐂𝐚𝐝 , 𝐏𝐓𝐒 , 𝐋𝐎𝐋 , 𝐅𝐢𝐟𝐚 , 𝐂𝐅 , 𝐋𝐚̣̂𝐩 𝐭𝐫𝐢̀𝐧𝐡 ............<br /> ↪️ Ae inbox để được tư vấn ngay nhé !!!<br /> -------------------------------<br /> 𝑯𝒂̉𝒊 𝑷𝒉𝒐̀𝒏𝒈 𝑪𝒐𝒎𝒑𝒖𝒕𝒆𝒓 - 𝑻𝒉𝒆̂́ 𝒈𝒊𝒐̛́𝒊 𝒄𝒐̂𝒏𝒈 𝒏𝒈𝒉𝒆̣̂ 𝒕𝒂̣𝒊 𝑯𝒂̉𝒊 𝑷𝒉𝒐̀𝒏𝒈<br /> 🎁 Tặng ngay Combo Quà tặng or Voucher #200k<br /> ✨ Hỗ trợ trả góp ngay +Đổi mới 15 ngày đầu+Free phần mềm ,vệ sinh<br /> 🏡Địa chỉ : 82-84 Quán Nam, Kênh Dương, Lê Chân, Hải Phòng<br />  ☎ Hotline : 0981.919.595<br /> 🌍 Website : <a href=\"https://l.facebook.com/l.php?u=http%3A%2F%2Fmaytinhhaiphong.com%2F%3Ffbclid%3DIwAR3PSVqmxqy34Eu3jDJbbZ0aRykOfPSNW4YDWJr2iq5_csqFUNtGWFNXeQc&amp;h=AT2ouApSINMd1y3NhsXV9AmiWbo1wQN8y5TtE_Bdtt-RUvbdBWHtVeqy5LsDNzErBNRGxoGNXILCp9mIc1O2YdIJDi2MwfK_tkyQh3ofqT2H9QAWD_WvsEPpU40Q2tbUp46FPzfEww\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">maytinhhaiphong.com</a>"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Trung Tâm Laptop Hải Phòng",
                            "disclaimer_label": null,
                            "page_like_count": 5502,
                            "page_profile_uri": "https://facebook.com/100091314824136",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712473200,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "923793355956691",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 286610277742618,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "107189848084236",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Trung Tâm Laptop Hải Phòng",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120207113254550345",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": null,
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Vị trí của bạn ở đâu?\"},{\"title\":\"Bạn có thể kiểm tra giá sản phẩm được không?\"},{\"title\":\"Tôi có thể mua hàng không?\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"user_edit\":false,\"surface\":\"visual_editor_new\"}",
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t42.1790-2/10000000_1378554192795764_5717810861852294686_n.?_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeF1zI7CpiDtbupmtKSiw1Avaq-bI_VS6Fhqr5sj9VLoWGWCXdPZXqrghNsJTZr0_EJIeQwrtpSJMxADxn6nUsR6&_nc_ohc=t-0rpPPt_YEAb7NgVez&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfBP-g9CHlbvl6eJioS486wUuM82ul8vi2lthXhGs9S9ug&oe=6622CD98",
                                    "video_sd_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t42.1790-2/432247711_635940392013956_5612273081088404429_n.mp4?_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGAXwy6dJnXJVYdDpl3KHvHMbBKd4g7-loxsEp3iDv6Wko2esugXaqfR9r54v2dAQDljeYobQA5oE3Mwgf8MMhs&_nc_ohc=ri3fTuqEJcEAb5dh886&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfDBsR1Hi-_x_83GA_vGC4cO7I50Oeaw4-d9j_dY00ySog&oe=6622D2D5",
                                    "watermarked_video_sd_url": "",
                                    "watermarked_video_hd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.35426-6/431503106_2890863691053793_9205923553605420097_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHoWvITNfwhbqCFOawR1ZVEpD2aNGYriJykPZo0ZiuInCtM9CGBQ0dsCUCXogBurZYeo35jQdxKWlk21wEM2uY3&_nc_ohc=RL9Fye4xhToAb5zzeWr&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfCyfiIfvWx5ziCEEuQVHHIE7Wn9CZL1csrShXTG-7KzJg&oe=6622AF07",
                                    "video_caption_urls": {
                                        "vi_VN": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.2093-6/432613429_780073450258217_3266781318551545093_n.srt?_nc_cat=106&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeE88irzpMwXiZkJqPuOqgtX6QtqckRWXBLpC2pyRFZcEnMPAavjp9s4Y_vtiXa6PIZrxk8cHuEK_7NNNeqmUGRl&_nc_ohc=BHtfaPrcwgMAb6x81Dj&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfDJG63WnbgmQd88y-7GU0cqnskDr-P_4UsqeIAdRxVJ6w&oe=6622C140"
                                    }
                                }
                            ],
                            "creation_time": 1710339698,
                            "page_id": 107189848084236,
                            "page_name": "Trung Tâm Laptop Hải Phòng",
                            "page_profile_picture_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/431223229_1916389665445212_6982630601465317611_n.jpg?stp=dst-jpg_s60x60&_nc_cat=106&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeER665oFztOhrX8BZHaw_sIL4aulUaTmtUvhq6VRpOa1fc1u42AUXyAsQe4LVu2i6zNmELChF690SCwZLcw-p5u&_nc_ohc=G73_N3eEOxsAb5Py1V0&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfDLoSyQgHeCTVjXeAI_sy5WKMV7iRJnn99ei9_iPjGkJg&oe=6622C799",
                            "page_categories": {
                                "200600219953504": "Shopping"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Trung Tâm Laptop Hải Phòng",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.35426-6/431170575_900439511763326_6265666422083550042_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeENS7qKg62zfwKQBpG1iDSuMw_NPjRj3CMzD80-NGPcI_bfA5ZtmsS7GGPFfjkAipuh2VisoQf5Btb3L6x38a1D&_nc_ohc=DLINF0rRtSoAb6S6O3M&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfAqJYEvDUsCXh0yzH3CE4GxDUdj32y8Vrj_uhgwcRMV_A&oe=6622DD28",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "HP Envy 1030 G3 ( i5 - 8250U  / 8G or 16G / 256 SSD / 13&#039; FHD cảm ứng ) laptop cao cấp chỉ hơn #8trxxx #hp1030g3 #elitebook #reviewlaptop"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Trung Tâm Laptop Hải Phòng",
                            "disclaimer_label": null,
                            "page_like_count": 5502,
                            "page_profile_uri": "https://facebook.com/100091314824136",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712559600,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "446523464431419",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 422688833779383,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "107189848084236",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Trung Tâm Laptop Hải Phòng",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120207751291140345",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": null,
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Vị trí của bạn ở đâu?\"},{\"title\":\"Bạn có thể kiểm tra giá sản phẩm được không?\"},{\"title\":\"Tôi có thể mua hàng không?\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting\":false}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting\":false}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting\":false}},\"user_edit\":false,\"surface\":\"visual_editor_new\"}",
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t42.1790-2/10000000_1547920679384053_5826830891367659506_n.?_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeG8BQ02V_B6f-zxMPbuhN5PGVWykxzHO4IZVbKTHMc7grEOtSLfmhetSmx0PHv5MYEunWVN0AYAakLG0XKDRyw1&_nc_ohc=GGA7TXBoCDoAb7V86QY&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfATKCvtIvs4Qn2oMCCmJYqMazF5xNH18j2qUT6_t6_eIQ&oe=6622D191",
                                    "video_sd_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t42.1790-2/434514933_451434313974340_1933527069903356234_n.mp4?_nc_cat=100&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGS2ju7o1ZzQF3om9cXHlbC_JJyquS6jnb8knKq5LqOdnltp9xlS2A4bNejcpdendynCMXqi-vdE0ACVbZdHmqv&_nc_ohc=m28QPj-wQxgAb5riUp7&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfB-EhnCX5ZCHAle3Po2WAukXQjUufGAWnO3aZpelPdkcA&oe=6622C639",
                                    "watermarked_video_sd_url": "",
                                    "watermarked_video_hd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/434569200_1461411491148349_7343303147227625486_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHhOvZ1rbz9UPzrsPOjXYbxAaX0ul6wBuQBpfS6XrAG5H8cxIwkRas6XKqYrfJh86ImU1x99IDugxhi5iMPmODV&_nc_ohc=0pBLYn_5_ZkAb6pePvF&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfASSHBUJ0f0Sui3DUDQ88Up0L8M0vQbSKrbnfDNXziemg&oe=6622D6C4"
                                }
                            ],
                            "creation_time": 1711680565,
                            "page_id": 107189848084236,
                            "page_name": "Trung Tâm Laptop Hải Phòng",
                            "page_profile_picture_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/434563490_345325127974531_1406091298246500131_n.jpg?stp=dst-jpg_s60x60&_nc_cat=103&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeH5g1M7m-owG1x3bQkLrWEEmBxt-Vuwn5-YHG35W7Cfn5eRpaSPFAvpN0RyYCMj9bRkPFE2lHOlkUjKHogPS0ki&_nc_ohc=diOdn-FhmEoAb5R9sG3&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfC8VBBQiD2stvMan7O8KKK6Are5KdsShhALxx36x2iPmg&oe=6622DAF0",
                            "page_categories": {
                                "200600219953504": "Shopping"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Trung Tâm Laptop Hải Phòng",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/434295928_740596548263291_2836022789220568109_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGfpSDxIBA384vTIyGOsaFletsniqcsG3J62yeKpywbch5AAzqkYBRat7nzuLNvoxXM57dELNYDzl6QE653a_Z0&_nc_ohc=jOs1ZvAw4XYAb4WebiL&_nc_oc=AdgGGRX7rzdJSXqbpZUJVRFPZA55GWbZqhxxG0gEn-8TE-SbWVQ8V4DIVpXXd64ZroE&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfBOMHwsxDXfgFuMKOhT3g0KEjvGYBARDF9tVDW8bqcp6Q&oe=6622D2D9",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "Dell Latitude 7400 2 in 1 ( i5 - 8th / 16G / 256 SSD / 14 &#039; FHD Tuoch ) siêu phẩm hơn #9Tr Ae không thể bỏ qua!!! #delllatitude7400 #dellcamung #Latitude"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Trung Tâm Laptop Hải Phòng",
                            "disclaimer_label": null,
                            "page_like_count": 5502,
                            "page_profile_uri": "https://facebook.com/100091314824136",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712127600,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "948274107017492",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 353878347008379,
                        "currency": "",
                        "endDate": 1713078000,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "107189848084236",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Trung Tâm Laptop Hải Phòng",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120207702865240345",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": null,
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Vị trí của bạn ở đâu?\"},{\"title\":\"Bạn có thể kiểm tra giá sản phẩm được không?\"},{\"title\":\"Tôi có thể mua hàng không?\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting_text\":false}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting_text\":false}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting_text\":false}},\"user_edit\":false,\"surface\":\"visual_editor_new\"}",
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "",
                                    "video_sd_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t42.1790-2/434511773_957313586103978_5465051704748547450_n.mp4?_nc_cat=103&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFyKzQrwhEZaaYX8R5QQIVdrSqXltMARwGtKpeW0wBHAWmGQ_aSMTDeu5P2ey_xeLBPYTi0AAehUnEYcfNsazA4&_nc_ohc=duA_zDUbLRsAb5_PskQ&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfB57l0ZyNhhsg3fhctB1NQFWiYDNR--bE1wg0z1wqwTRQ&oe=6622C036",
                                    "watermarked_video_sd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/434175687_1006916447732484_4482572133610472911_n.jpg?_nc_cat=103&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGaOg43aTxrmrsvzHSv0Mfkqlb5uS-OBQyqVvm5L44FDEC0IIjIg5pVBsUyElNbgTOaLbAid9XfsZYQpIVGu_6p&_nc_ohc=c10VWodZVVAAb5Qn_pO&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfAlTrjgYTHwHZm5uDmqM_eDuiqkfX6yjkozrldsLiu7Vg&oe=6622AC51"
                                }
                            ],
                            "creation_time": 1711592801,
                            "page_id": 107189848084236,
                            "page_name": "Trung Tâm Laptop Hải Phòng",
                            "page_profile_picture_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/434177859_1039171790990313_1966334266338276938_n.jpg?stp=dst-jpg_s60x60&_nc_cat=106&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHrSZmQtGuoCU-YzXTkAGjfTqB05w61d-hOoHTnDrV36A1zF4LS8OyS_v4_alM9QZrw5YzmV4zCV8h2qL37Hs9t&_nc_ohc=2YS3pmPOHBcAb5OtQaB&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfBBfl5TyCH8J4Xn9w2ocLoompIxD4EP2RprepsOekgVBQ&oe=6622BD69",
                            "page_categories": {
                                "200600219953504": "Shopping"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Trung Tâm Laptop Hải Phòng",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.35426-6/434216655_728028046169104_8542822400814638515_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFF-SSi0IcCoWmaZRwjskOXnuXP6KPq2OWe5c_oo-rY5TPyVl38QhJ2l2c1LMinvwijjg9Ja6TsNQBoyf0Vu6t5&_nc_ohc=Vjj6MNYA3mkAb5g2mDc&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfATL5PXZQcMLj7BD4fefLnjiyicl0yQveY-tTH-s1Y1VA&oe=6622D2A9",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "😍 𝐔𝐧𝐛𝐨𝐱𝐢𝐧𝐠  𝐌𝐚𝐜𝐛𝐨𝐨𝐤 𝐀𝐢𝐫 𝐌𝟏 𝐦𝐚̀𝐮  𝐆𝐫𝐞𝐲 𝐬𝐢𝐞̂𝐮 𝐜𝐮𝐨̂́𝐧 𝐡𝐮́𝐭 <br /> Cảm ơn b khách xinh đã tin tưởng và ủng hộ #HPC 🥰🥰<br /> 👉 #MACBOOK_AIR_M1_RAM8GB_SSD256GB_13_RETINA<br /> <br /> ↪️ Ae inbox để được tư vấn ngay nhé !!!<br /> -------------------------------<br /> 𝑯𝒂̉𝒊 𝑷𝒉𝒐̀𝒏𝒈 𝑪𝒐𝒎𝒑𝒖𝒕𝒆𝒓 - 𝑻𝒉𝒆̂́ 𝒈𝒊𝒐̛́𝒊 𝒄𝒐̂𝒏𝒈 𝒏𝒈𝒉𝒆̣̂ 𝒕𝒂̣𝒊 𝑯𝒂̉𝒊 𝑷𝒉𝒐̀𝒏𝒈<br /> 🎁 Tặng ngay Combo Quà tặng or Voucher #200k<br /> ✨ Hỗ trợ trả góp ngay +Đổi mới 15 ngày đầu+Free phần mềm ,vệ sinh<br /> 🏡Địa chỉ : 82-84 Quán Nam, Kênh Dương, Lê Chân, Hải Phòng<br />  ☎ Hotline : 0981.919.595<br /> 🌍 Website : <a href=\"https://l.facebook.com/l.php?u=http%3A%2F%2Fmaytinhhaiphong.com%2F%3Ffbclid%3DIwAR1CLBed14Z2pGKKMCd3Enjx2dOlJ-87NXuHW8o4QVRPgsCh0vh2iWMb0-k&amp;h=AT3hpKkNoqHMvwGfYxO8wZsbhAjb86uUxQyObrfoMkKeEFbeE7M-m_H5JCFJmG-C29l3DeUOVTIkLwxZlGcctL19_6-UuLK9qFdmbOyThfcfVRQ1HlpHldcP1lGNtiBIuOneMQVyEA\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">maytinhhaiphong.com</a>"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Trung Tâm Laptop Hải Phòng",
                            "disclaimer_label": null,
                            "page_like_count": 5502,
                            "page_profile_uri": "https://facebook.com/100091314824136",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712127600,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "941081574175215",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 1614793499276311,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "107189848084236",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Trung Tâm Laptop Hải Phòng",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120208271496300345",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": "Chính Sách Mua PC _ Laptop tại Hải Phòng Computer",
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Vị trí của bạn ở đâu?\"},{\"title\":\"Bạn có thể kiểm tra giá sản phẩm được không?\"},{\"title\":\"Tôi có thể mua hàng không?\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting\":false}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting\":false}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting\":false}},\"user_edit\":false,\"surface\":\"visual_editor_new\",\"ai_generated_welcome_message_impression\":false,\"has_ai_generated_welcome_message\":false}",
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t42.1790-2/10000000_941081627508543_4058755284355384241_n.?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGpr92vcqLWo1AkXDDGwCU2W_WBsIv3aVNb9YGwi_dpU-7D4ivYlBZUZt1tUeuewf1x8OTmtTAZkkNDePP__aUa&_nc_ohc=jmdgXIdK170Ab6JJQos&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfAifAhY7XeREH2l6StU1CbktSf9TWSY0I9ToFBddguDBw&oe=6622D15D",
                                    "video_sd_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t42.1790-2/435850532_1120229689016149_6713742108482099763_n.mp4?_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEXwGm2B_U4OPoE6SCKWrerISa-IWctvBMhJr4hZy28E8e-echZvvTzzgtTUnEaVVX86gfcua-l1kCSrm2ALrT1&_nc_ohc=KjKrHjIbJ0oAb49KKR8&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfCioArJpA7KB-vuGBj7PSeXuyZByUb-EMgD7zNECpnddg&oe=6622B042",
                                    "watermarked_video_sd_url": "",
                                    "watermarked_video_hd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/434481900_738351541791489_1908672898761864528_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEAA3OHsvAcjfqjMX0MEaD3CN76Ly0EN7MI3vovLQQ3s5YStVvY5xt04eD4qS6E8UHsCUau3iaEghEFDu2xm266&_nc_ohc=RUCIUOroIkoAb524Ju6&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfCtZTdn9Ga11YjQ4cC_l5IrsgXwtLSRKmlQUUJX03lI3w&oe=6622CC0D"
                                }
                            ],
                            "creation_time": 1712745719,
                            "page_id": 107189848084236,
                            "page_name": "Trung Tâm Laptop Hải Phòng",
                            "page_profile_picture_url": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.35426-6/434408528_1454126288537242_5195459165481343394_n.jpg?stp=dst-jpg_s60x60&_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeE3ZxS2YVJ9BDmUctUlaYBSxsJiBDuDiUjGwmIEO4OJSMrDNBGPv3F9OCHVbOpsNMXe-ndBpXjZWxzc3JoKJDQT&_nc_ohc=G0k0d0N_TjwAb4nLlDn&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfDeNWzBIFHxHljZqplmnxyS6hTyzbUsqJd3yhJ97JnKXQ&oe=6622BAF6",
                            "page_categories": {
                                "200600219953504": "Shopping"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Trung Tâm Laptop Hải Phòng",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/434469743_723789166568320_367050245141902639_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHK7aVJeePFNWpTrIKgybhtEDEK7ftwwSsQMQrt-3DBK7-JTXc_qLg0PLXvH-TSiRmYv-qiP8kggga4uLWPsxaS&_nc_ohc=SlKaztXN-QQAb5LAwiz&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfDWhHlM7v-U-MVhg_bLcvfzNxKpZC-xhklkBOOnyudb3Q&oe=6622CC97",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "⁉️ Mua Laptop-PC Ở #haiphongcom Bảo Hành Như Thế Nào?<br /> ------------------------------ <br /> 𝑯𝒂̉𝒊 𝑷𝒉𝒐̀𝒏𝒈 𝑪𝒐𝒎𝒑𝒖𝒕𝒆𝒓 - 𝒏𝒐̛𝒊 𝒎𝒂𝒏𝒈 đ𝒆̂́𝒏 𝒔𝒖̛̣ 𝒂𝒏 𝒕𝒂̂𝒎 𝒗𝒂̀ 𝒕𝒊𝒏 𝒄𝒂̣̂𝒚 𝒄𝒉𝒐 𝒎𝒐̂̃𝒊 𝒔𝒂̉𝒏 𝒑𝒉𝒂̂̉𝒎 𝒃𝒂̣𝒏 𝒎𝒖𝒂!<br /> 🛡️ Chúng tôi cam kết đem đến dịch vụ bảo hành tốt nhất với các chính sách linh hoạt và tiện ích:<br /> ✅ Bảo hành dài hạn: Mỗi sản phẩm bạn mua tại Hải Phòng Computer đều được bảo hành theo các điều kiện cụ thể, đảm bảo sự an tâm và tin cậy.<br /> ✅ Chăm sóc khách hàng 24/7: Đội ngũ nhân viên chuyên nghiệp và nhiệt tình luôn sẵn sàng hỗ trợ bạn mọi lúc, mọi nơi, để giải đáp mọi thắc mắc và giải quyết mọi vấn đề.<br /> ✅ Đổi mới sản phẩm: Trong trường hợp có bất kỳ sự cố nào xảy ra, chúng tôi cam kết hỗ trợ bạn đổi mới sản phẩm một cách nhanh chóng và thuận tiện nhất.<br /> 📹 Hãy cùng xem video để hiểu rõ hơn về chính sách bảo hành của Hải Phòng Computer và đừng ngần ngại liên hệ với chúng tôi để biết thêm chi tiết và đặt mua các sản phẩm công nghệ cao cấp!<br /> 📞 Đừng chần chừ, hãy để Hải Phòng Computer chăm sóc nhu cầu công nghệ của bạn một cách tốt nhất!<br /> ====================<br /> Hải Phòng Computer chuyên PC Văn Phòng - PC ĐỒ HOẠ- Máy Xeon - PC Game Giá Rẻ - PC Tản Nhiệt Nước - PC AMD -Laptop<br /> ---------------------------------<br /> • Địa chỉ: 82,84 Quán Nam - Lê Chân - Hải Phòng<br /> • Hotline: 0899.256.166<br /> • Website: <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fhaiphongcomputer.vn%2F%3Ffbclid%3DIwAR35XgRogGoxtT2QC4fogm1gL8ZN5HtDco_3Z_SmSSneyaaQKNjoIcTrcuQ&amp;h=AT3Sq1oRDu4x4mO96ri8rH0tovBvxtUF1A2WnE3PTw7clIDEUQxJfzLU3jm8xR8CvLirD6flcMKiWZnsMHQFSYXoT9EOy-DfdrKcyUTsRUxZEyetYmCnmY8IE797fQnhdG8O3mEDow\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://haiphongcomputer.vn/</a><br /> • Tiktok: <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fwww.tiktok.com%2F%40haiphongcomputer.vn%3Ffbclid%3DIwAR1VnsA0g1Wtw4SvoPe87t0NWBFrSDxuAe6t2kfrkaVDMcLZbCYYnmWCzRk&amp;h=AT04NG2Hajo9kS_9UM6e1XZ8nRGqD54Jvg52Yg_whZWBG_2lEkrevYNFFU6rYYRVxbyLKimd6ObH2PcQmmUOr5FjR_nlPaiwN2kmfahErFlfz8ALKgdlgSKW79ykIE0P_q40Tqi3DA\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://www.tiktok.com/&#064;haiphongcomputer.vn</a><br /> #HảiPhòngComputer #BảoHành #ChínhSáchBảoHành #DịchVụChămSócKháchHàng #CôngNghệ"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Trung Tâm Laptop Hải Phòng",
                            "disclaimer_label": null,
                            "page_like_count": 5502,
                            "page_profile_uri": "https://facebook.com/100091314824136",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712732400,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "1119286179109337",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 976822434019725,
                        "currency": "",
                        "endDate": 1713078000,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "107189848084236",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Trung Tâm Laptop Hải Phòng",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120208192386740345",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "multi_images",
                            "title": null,
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": null,
                            "images": [
                                {
                                    "original_image_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/435712305_432295792812814_5780309037611391128_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeG1dIYJPR7-Wo_CD0Rj4lG_P_OOrLumRf4_846su6ZF_tBsLUfGVpkI76AziRmO05dUy-ro51dav_19oO-IF_vQ&_nc_ohc=WQc7mAzdeAcAb7kkQM7&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfAVbNw2LUBEsiZM3b26YO1NuDWu7audBmFFlOBlopUFaQ&oe=6622DC4B",
                                    "resized_image_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/435471911_1807927463366788_8600173128041633530_n.jpg?stp=dst-jpg_s600x600&_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFX_Vn7J_Wc1XBwE8_E4a8YRLxxyRPJmB1EvHHJE8mYHep1v8_RQpOhXEibmHhfrrHK9FZkuHi5HbsfqYDSozj2&_nc_ohc=K_0SpItx-AoAb7YEJVS&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfD6843NxeNH7qctQ-oXqYJO5JFYOlvtvHM8y4tqYlfoNQ&oe=6622D73E",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.35426-6/435462527_879495773978015_4104877842610460618_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGFxhsZEW502FsODxUWU-_VxOmB55EC_UrE6YHnkQL9SuLyFjC19WFnpxc4vbPE25H3VY9JlnN4OAwibiOSX3dN&_nc_ohc=GHHhlacndCYAb7DeBO-&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfB7B37jovAsGc_KCo2pRMHh6oUG-2sNn4taP0C93rEKFQ&oe=6622B34F",
                                    "resized_image_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/435460823_3721977764791185_600598288845953664_n.jpg?stp=dst-jpg_s600x600&_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHpcnEC1F5KfeQNzBh52kMJPI__gtgY9G88j_-C2Bj0b6FVjMRRKkxOiorYKoho-aBlpExyfRuAPIVygSE5CcHE&_nc_ohc=rR7Y2fI0ujkAb4nbgVo&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfAnBPe_WE0GmxSuvNgWWayu1EtkERyB1H4gvPvbHP15wg&oe=6622A53E",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/435411057_1606066910141347_7644736939139718799_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEn54mnhXMJ1TvRVpJizWfmKQy52cAmw6YpDLnZwCbDpgVSo3qPlK_hmKbbujDPBoWMc4X4IYNPqznADTthqhuz&_nc_ohc=xEr92ZyFXL4Ab6eWPf2&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfAlUWtheHkH7wmM5yosmN3EXNd_YlfuQIBOSzrXk4avJg&oe=6622A63E",
                                    "resized_image_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/435480447_751304383773328_1325451375042629988_n.jpg?stp=dst-jpg_s600x600&_nc_cat=100&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFT5wfDPQVpNFJLinPtwTa2BphfQmOQHKsGmF9CY5Acqw1ytJWcPUcWjfq9o9R1i99thNtNFJy9DcY20-3Mk0FT&_nc_ohc=XBHyWorzaL8Ab7ErM64&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfAh_cuhHdPl5zakgTc1_z1E39s4R_VpQI_M8lXR1mKA7w&oe=6622AC29",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/435484913_7412918572121155_7610987673168293224_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeF2aGzHt2J3VxehKV0GCrrONHkxNyckj4Q0eTE3JySPhCuPW8SL8kbT_3tgpYgwCke1-H-bmPLW44i_wyAuptki&_nc_ohc=KmWC0QYDEwEAb4D-5aC&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfBGkntGkQ4-H6AETnKGJdgXoVSI08NKDXaGYgvFLjbpVw&oe=6622BCF8",
                                    "resized_image_url": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.35426-6/435708380_414909417966981_5496963814261499543_n.jpg?stp=dst-jpg_s600x600&_nc_cat=101&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEu5XsPTDa1zO4j6Onhto-IMMb6O5YtvKwwxvo7li28rNfCs6L_3MZjMpxx7SKkHb3Fjbk7vq1JIQvfmrCOlUU-&_nc_ohc=tPPkpuBb6qcAb5jC0B6&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfC7XUBX0Gq_I9W9tBcXTReWJlGQmMauIscFlYh9ReNqTA&oe=6622C2BD",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/435690757_834372938466466_772626875486085553_n.jpg?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeH7tc5OutIIx7-8tjfgfR0F4qe5jB38dzzip7mMHfx3POwOU-5sxZ3sd2rU--Fpxpcv_lY0H84Ysogu7OW2k5Dl&_nc_ohc=iDEN8s_35QMAb6-AC-i&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfBX2ScIRPs2EKIicekx6IaA2_y4BRotEBaZxjRZ6zjaZw&oe=6622DC32",
                                    "resized_image_url": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.35426-6/435688871_1451516539076762_3496386586682543073_n.jpg?stp=dst-jpg_s600x600&_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHg3i2tio-QqW9b5epNFXrqYGjvh1NyLNJgaO-HU3Is0tqr3z4ul4zh8L0Kqm47oJMPr80mIEY_KpBoVWC-J46R&_nc_ohc=_hkVXb44HrYAb4b9Tf4&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfBhTbGqBxEDxCK0CYdWD-yRadFEPwN8xoO5hyQwjKt86g&oe=6622D5CD",
                                    "watermarked_resized_image_url": ""
                                }
                            ],
                            "videos": [],
                            "creation_time": 1712599550,
                            "page_id": 107189848084236,
                            "page_name": "Trung Tâm Laptop Hải Phòng",
                            "page_profile_picture_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/435417143_743809987903631_8386941812347898071_n.jpg?stp=dst-jpg_s60x60&_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHtF_kqJIJgKNPL1T73zsjqG6Kp2j2d7EQboqnaPZ3sRBUyqiP8rQhfyIlgxPcKhzFhrww1RTKuex8In90_0cF2&_nc_ohc=XspMTLUpPJUAb7ETFG4&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfBIZp0v_FXpKPdwitIhxTU31kRUtX21nmFW_ZExR02GPQ&oe=6622ACF9",
                            "page_categories": {
                                "200600219953504": "Shopping"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Trung Tâm Laptop Hải Phòng",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.35426-6/435426747_1621797418630334_8551804071758043766_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFQqXpqraxLrVHPENqMHcm3WKPHLlRtjHFYo8cuVG2McatKbzm67jdRGUg7MfqOAxCVZ9t0kVFn4md7AaEB3jWC&_nc_ohc=NJsIMOjGxZEAb4a7oBW&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfBU3k8bIEvLTlg7Z1k-04EwGeaLdKKsMnKn_HYNNdh12Q&oe=6622C5F8",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "❌ XẢ KHO CỰC SỐC  5 COMBO PC TIMBER GIÁ HỜI TẠI #haiphongcom<br /> 🛠 𝐂𝐚̂́𝐮 𝐡𝐢̀𝐧𝐡: 𝐢𝟓 𝐠𝐞𝐧𝟏𝟐/ 𝟏𝟔𝐆𝐁 𝐑𝐚𝐦/ 𝐕𝐆𝐀 𝟑𝟎𝟔𝟎 𝟏𝟐𝐆 giá #16tr390k<br /> 🎁 Tặng kèm combo: Bàn phím + Chuột máy Máy Tính<br /> 💵 Có Hỗ Trợ TRẢ GÓP 💵<br /> ------------------------------<br /> - CPU I5 12400F T NEW  (Bảo hành 36 tháng)<br /> - Main B760M 2 khe DDR4 new (Bảo hành 36 tháng)<br /> - Ram 16gb trắng d50 (2*8) DDR4 (bảo hành 36 tháng)<br /> - Nguồn 750W (Bảo hành 36 tháng)<br /> - SSD 256GB (Bảo hành 36 tháng)<br /> - card rtx colorful igame 3060 12g ultra white oc l - v cũ (Bảo hành 3 tháng)   <br /> - tản khí CT AIR03 trắng (Bảo hành 6 tháng)<br /> - Vỏ centaur timber trắng to + 5 fan HALO + dây nối 3 màu<br /> <br /> ↪️ Ae inbox để được tư vấn ngay nhé !!!<br /> ----------------------------------------------<br /> Ư𝐔 𝐃Ã𝐈 𝐊𝐇Ủ𝐍𝐆 𝐊𝐇𝐈 𝐌𝐔𝐀 𝐇À𝐍𝐆 𝐓Ạ𝐈 𝐇Ả𝐈 𝐏𝐇Ò𝐍𝐆 𝐂𝐎𝐌𝐏𝐔𝐓𝐄𝐑<br /> ✅ Miễn phí vệ sinh và bảo dưỡng máy tính trọn đời máy<br /> ✅Miễn phí bảo hành phần cứng tại nhà<br /> ✅Miễn phí đổi máy trong 1 tuần đầu nếu dùng máy không ưng ý hoặc muốn đổi lên cấu hình cao hơn.<br /> ✅Ngập tràn quà tặng đi kèm khi mua PC hoặc Laptop tại Hải Phòng Computer<br /> ✅Tất cả linh kiện máy tính đều nhập chính hãng, bảo hành lên đến 36 tháng.<br /> 👉HỖ TRỢ TRẢ GÓP:<br /> <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fhaiphongcomputer.vn%2Fhuong-dan-mua-tra-gop%2F%3Ffbclid%3DIwAR3hJm0myEcuzgkxbuNcsXOetzzFIX9zGY2aO1Uycnuroej09Drb4iUuue8&amp;h=AT05e23HBvrc7_Zdtie-MfErl6q5Y4x10kaW6sWomWmvr0_LjF4oTCY9ni6y32-0C3pCNfiTpdpvEIFQ_heE_i3bWMVaZYAAcCN-pR7LaJqXHG33mKeOGducSnHznpFOlQ3XHI6ui5pFwzU2uEz09r4\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"async\">https://haiphongcomputer.vn/huong-dan-mua-tra-gop/</a><br /> 👉CHÍNH SÁCH BẢO HÀNH:<br /> <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fhaiphongcomputer.vn%2Fchinh-sach-bao-hanh-san-pham...%2F%3Ffbclid%3DIwAR0fDzTL8VzJSnlnyvC0lbvMB0ZTY0_1lc4K2btoZdMp2lK1vtrfDCn6900&amp;h=AT27lW5fhz-qS_Pig0Mn-UgsvHsjt516ga5biuEHq3BtRY5tBQd1j19sHMJiMMC3_yJfXk9yvxu3ym7HkaJu3WycOOPsfcs_AlT2wL3PCD6frp4_X18hkXZ-9JdVYZ-BCrPPOT7QaXKQSXoocEdCdk0\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"async\">https://haiphongcomputer.vn/chinh-sach-bao-hanh-san-pham.../</a><br /> 👉CHÍNH SÁCH VẬN CHUYỂN:<br /> <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fhaiphongcomputer.vn%2Fchinh-sach-van-chuyen%2F%3Ffbclid%3DIwAR2Ldn2x7SfoOqwypRWju32iEhdIxifa4Gw77APZPGEZ637bjCNhS3er-m0&amp;h=AT0xx-A36qw7R7GmWDdi3OJNsHJvsdjbEI3UqHvQpLxwOZ0Pi7DdDXILfm-sTLg4T8D4qYBd1JekbN7Rm7HiJzOR5o8ElRZOt9LGR1OGu85ZLkzWic8EdBQqtYILs9xcK_zi5vEb6Q\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://haiphongcomputer.vn/chinh-sach-van-chuyen/</a><br /> <br /> 🏡Địa chỉ : 82-84 Quán Nam, Kênh Dương, Lê Chân, Hải Phòng<br />  ☎ Hotline : 0981.919.595<br /> 🌍 Website : <a href=\"https://l.facebook.com/l.php?u=http%3A%2F%2Fmaytinhhaiphong.com%2F%3Ffbclid%3DIwAR3jzreTaneQq73JApM4wgXBAUBjVGjFukffhm004O7YuPYIZDEVkEPGr6o&amp;h=AT2EvGKA7OlYbGUtdDvQsw4MjSgUFjjvEgJ5V6he1fCZrSSBsenGMUJi-zpf15ryfqXn2FbRGGZj5DfcmHcNEuVYVKIjQB2BBuRNwSv7gbM4_gXeCEBtsDfxVK_kZm0nOSUo8by-Og\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">maytinhhaiphong.com</a>"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Trung Tâm Laptop Hải Phòng",
                            "disclaimer_label": null,
                            "page_like_count": 5502,
                            "page_profile_uri": "https://facebook.com/100091314824136",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712559600,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "7341809959264905",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 1125684251890671,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "107189848084236",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Trung Tâm Laptop Hải Phòng",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120208191704270345",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": "DELL INSPIRON 5310",
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": null,
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t42.1790-2/10000000_1392530074800896_2226751326184439350_n.?_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeG1yWd7SEgLCVc-j5i1sIYa-guyV8Tt3Ev6C7JXxO3cS3jVPNkLuGe-vfRCVkAbXjZ340aNzhQGnHA7QwJ7CPjp&_nc_ohc=mDzALca3gHsAb654JE8&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfDoZPfPq8-E-F_cXsQvzZPaokzlXkxxWKWnrOh9kaXhvQ&oe=6622CDB6",
                                    "video_sd_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t42.1790-2/435540445_737849561670737_1048810956959649257_n.mp4?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHixedEH93BsTTnqCG_M2Zrn2aJpMbMp0-fZomkxsynTxMDa3HBg1JkJH9zE7kKhXvm3IDferqgIfyAyGjzjLzV&_nc_ohc=DZLi-gffcqAAb6vDGUE&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfAZDh6IIR-lEM7IeTTjrkc5p-m3KUOcKH7yhRIzHdnhNg&oe=6622C4D9",
                                    "watermarked_video_sd_url": "",
                                    "watermarked_video_hd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/436366065_350193387489991_5404564005632902526_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHmBGigCTGC9zn9qzTqXT5IqSD71tbtazypIPvW1u1rPCdr0itrLRIG_WJM8toUaEPrcfOj9yX4G3GwgpVb8jSQ&_nc_ohc=ceZznNl2gPMAb77UNgZ&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfBEXJSFmbIFqNmOzIbmrJDSRcDW1w-VXeRGKBezDfZlhQ&oe=6622C151",
                                    "video_caption_urls": {
                                        "vi_VN": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.2093-6/434780320_342707615482690_4745463547054821576_n.srt?_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeE4xEU5nR8er0TAckc4-Ub9w9lTTczYhyzD2VNNzNiHLDJQvqGtaiqJT_WYUt6PeOK0700YWClsOXw66N6Vs_0l&_nc_ohc=uqeICcb3PMMAb4r3vBO&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfCY0Q-oCWtVfcgg4EndufcUg8V6SMHahEsHAggbphpUnQ&oe=6622D138"
                                    }
                                }
                            ],
                            "creation_time": 1712598314,
                            "page_id": 107189848084236,
                            "page_name": "Trung Tâm Laptop Hải Phòng",
                            "page_profile_picture_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/426265611_1127513978387667_8595509903576736026_n.jpg?stp=dst-jpg_s60x60&_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGoDaxZxskjgmh1ADLcMUL6gjys8ItRbfCCPKzwi1Ft8LL0EyyIWnibmn18C_oUlRXIsSdtsLlJ8xhu9nLteVi7&_nc_ohc=2KGyf8VgVyUAb5-BOLM&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfCYtA_IH6ZVLKWVATGdatwCvLpXp-VOjKsVqtkbL6WEQA&oe=6622BA73",
                            "page_categories": {
                                "200600219953504": "Shopping"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Trung Tâm Laptop Hải Phòng",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.35426-6/436206437_1167258317605496_3712541482363728598_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFQNm-QfoFBG_4zsLdw8SXSUjpEHc79XFBSOkQdzv1cUGLx2IMwe2e3FF1R8WSTRClgXcqMOITA70ZT2Mtkl9zs&_nc_ohc=XcIFrL1h3sUAb7Yg1mx&_nc_oc=AdhZtLfUYkRG7UCiUw7ggV1YBsViOR7HbhFjbOJDg-PUJPjxt_B5NI80BkQopp4TWPM&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDWpBJHXuhI5j0Uapj3wy6TYOZVa4co7hTp_LUzQPOOxg&oe=6622C477",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "⚠️ ⚠️ HÀNG HOT  - GIÁ GIẢM CÒN HOT HƠN 📣<br /> <br /> 🔰 𝑫𝒆𝒍𝒍 𝑰𝒏𝒔𝒑𝒊𝒓𝒐𝒏 5310 | 𝑰5 - 11320𝑯 | 8𝑮𝑩 | 𝒔𝒔𝒅 256𝑮𝑩 | 13.3&#039;&#039; 𝑭𝑯𝑫 <br /> 👉 Chi tiết tại: <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fs.net.vn%2F2Kk7%3Ffbclid%3DIwAR1G0r0vRH8zrXI3bE4QZxnye8ZBnGGoRWpspmKlw2CUSkd9S2akCes_ZB0&amp;h=AT252o8GhFejlmrkREqisI8D6Qa3piqGlno386W9V_iJ-i2FwZOIZkdCjoHrKAH3q-kDFWfA-fmHu9msseUQWwIaqx-5_MbjLRncmNSAa6xCU2Gyor_zuXtZwx_9oz7-Zb4ljEfXRA\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://s.net.vn/2Kk7</a><br /> -------------------------------------------<br /> ✅ Là 1 trong những chiếc Ultrabook có HIỆU SUẤT ĐẶC BIỆT NHẤT  được trang bị CPU Intel Core i5 - 11320H (4 nhân/8 luồng) cân mọi tác vụ từ văn phòng cho tới đồ hoạ bán chuyên nghiệp<br /> ✅ Ngoài ra, máy còn được trang bị sẵn 8GB RAM/256GB SSD (có thể nâng cấp lên tối đa tới 2TB SSD) - những thông số LỚN NHẤT phân khúc<br /> ✅ Build kim loại cực kỳ chắc chắn, màu sắc sang trọng. <br /> ✅ Màn hình IPS 13.3&quot;, độ phân giải FullHD+, 100% sRGB đem lại trải nghiệm MIỄN CHÊ<br /> ↪️ Ae inbox để được tư vấn ngay nhé !!!<br /> ---------------------------------------<br /> 🎁 Tặng ngay Combo Quà tặng or Voucher #200k<br /> ✨ Hỗ trợ trả góp ngay +Đổi mới 15 ngày đầu+Free phần mềm ,vệ sinh<br /> 🏡Địa chỉ : 82-84 Quán Nam, Kênh Dương, Lê Chân, Hải Phòng<br />  ☎ Hotline : 0981.919.595<br /> 🌍 Website : <a href=\"https://l.facebook.com/l.php?u=http%3A%2F%2Fmaytinhhaiphong.com%2F%3Ffbclid%3DIwAR2kpcnGcbtyR7NjZVdvcegMIUVyGIYMxL4VQ_4pWFuRqryu0zkbRHp7YFI&amp;h=AT3Vp_3cPPGVvtYzqzluP-zYvu_1mcpYo0asZbxpMSBRK0DyPiBcdjF0-a7yzS1823G85Kc6ei40KEmnG0KeUnkcpGJKkMGEfP2YxuinmAzptUZojzbyE_8GFQ_MQsREVXpQxe-DzQ\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">maytinhhaiphong.com</a>"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Trung Tâm Laptop Hải Phòng",
                            "disclaimer_label": null,
                            "page_like_count": 5502,
                            "page_profile_uri": "https://facebook.com/100091314824136",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712732400,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "1370663277662610",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 819193713417756,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "107189848084236",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Trung Tâm Laptop Hải Phòng",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120208191807040345",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": null,
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Vị trí của bạn ở đâu?\"},{\"title\":\"Bạn có thể kiểm tra giá sản phẩm được không?\"},{\"title\":\"Tôi có thể mua hàng không?\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting\":false}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting\":false}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting\":false}},\"user_edit\":false,\"surface\":\"visual_editor_new\",\"ai_generated_welcome_message_impression\":false,\"has_ai_generated_welcome_message\":false}",
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t42.1790-2/10000000_1370663300995941_6215230013855527942_n.?_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFwXdKPcoBfuomhvpiiY0dMH4nuvApr_bIfie68Cmv9suT7Vyt4xpw4LmIrrXqj10NVwNGYnBRsXTbSYGAc8pfl&_nc_ohc=MRhWGGi6Q9AAb5VEF-J&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfBo4bfjmP6_cOLV8tP-2ci46CR3qdxbPMxVY6pd7S_yKw&oe=6622BAC5",
                                    "video_sd_url": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t42.1790-2/435526390_1693312144532854_8442319350434934631_n.mp4?_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFfP7qGLGuJA_aIc62_EuT8ygyx5UfA4zLKDLHlR8DjMmD0SB0Tgj5yQ5VzH3szdUWqMC-fObOoUc4ktwfLQF4C&_nc_ohc=BTz5U5Cc538Ab4kJ9C5&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfAI7qvSA9fnilOWWd6Dc1y4AfBULs-nIWdJYU8L6zHhfQ&oe=6622C22E",
                                    "watermarked_video_sd_url": "",
                                    "watermarked_video_hd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.35426-6/435003846_278280981943318_2195976950368130689_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeF1CLKEx-cPLa55VBJUr-HK6lS9mt9jcgbqVL2a32NyBrX9-lYwqvVbJS9unm63Ezvz98K15Dx5n52MMQM3wjWi&_nc_ohc=ncvMpuoxAO0Ab7qNf7d&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfCxOFqnQquOqjMbuNJDyV2kLwJNeVWrd3iruJhqG2Psyg&oe=6622C37C",
                                    "video_caption_urls": {
                                        "vi_VN": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.2093-6/435162858_268893366278287_2511003039635239860_n.srt?_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFok8D8s0RmoEbIvEN8pk-_rMTllxuUr7isxOWXG5SvuBt7fdhuRGXTdOmaaPX2Aa1Sk9Ar92qRBxB_dVbJcx3s&_nc_ohc=723IJqNUtXYAb6nq0v0&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfChEKGfI1NHI16etXnKn_csWHwqoIThOkJexVgFazOQzw&oe=6622C6C6"
                                    }
                                }
                            ],
                            "creation_time": 1712598476,
                            "page_id": 107189848084236,
                            "page_name": "Trung Tâm Laptop Hải Phòng",
                            "page_profile_picture_url": "https://scontent.fsgn2-5.fna.fbcdn.net/v/t39.35426-6/434652868_2061649474218884_2601880340355497507_n.jpg?stp=dst-jpg_s60x60&_nc_cat=104&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEXwbL-vVr5eozB1UJUk89Qu677S1UNUKG7rvtLVQ1QoYZ0L06GRRNuDCuzQ8n9bv7IuK03hX5h6PEBmfj-C-qs&_nc_ohc=hagnOvBr5E0Ab4c72sQ&_nc_ht=scontent.fsgn2-5.fna&oh=00_AfCBv1UEsfMRVVQ2aKTBpukj29ZGqFqRBWWhtzQ1EMrTHA&oe=6622AAC3",
                            "page_categories": {
                                "200600219953504": "Shopping"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Trung Tâm Laptop Hải Phòng",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/435063571_359554847083776_8847587513148089216_n.jpg?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHqpmvZb1N7-E56F0kdR38rm8kafx56xgabyRp_HnrGBj1xWpOIhlsD7DfH4WBythUQKI1wz4k2wgs-bT-uPxPD&_nc_ohc=qfif-Mw6ye0Ab5pqwn-&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfAQ6g6QQUjI6nz6nweJZEDu4GOkPCytuak8OBTT4iCSdg&oe=6622A6B2",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "⭕️❌ Xả kho 1000 chiếc Dell inspiron 5498 ( i5 - 10th / 8G / 256 SSD / 14&#039; FHD )  giá tốt nhất thị trường !!!! #dellinspiron5498 #dellvanphong #HPC"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Trung Tâm Laptop Hải Phòng",
                            "disclaimer_label": null,
                            "page_like_count": 5502,
                            "page_profile_uri": "https://facebook.com/100091314824136",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712559600,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "1157612915658078",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 1439990174064380,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "107189848084236",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Trung Tâm Laptop Hải Phòng",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120207563315380345",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": "Dell 5300 cảm ứng i7 giá giảm sốc !!!!",
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": null,
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t42.1790-2/10000000_709524454457105_3542067509559481495_n.?_nc_cat=106&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFSAR6mBj-ZRRhPzHztQOChr85vufL3Lgevzm-58vcuB0XlgDeTIAf_BNjf8NwFBkN-UBut6aEIFye99UUIBFCO&_nc_ohc=RSYzn8hNo1oAb6g3OKa&_nc_oc=AdhTTrkW6pPv3jS1tMkaGANUXsryGjxSia18cI5JuJj5S1isrV49SFLT2sANC9_1do0&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfBJXTuVO3qDWXWHAhUNsHLMAAA8c4t26aNl4fZgGcrMDQ&oe=6622BA6F",
                                    "video_sd_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t42.1790-2/434007876_753517906870210_2561559359633537901_n.mp4?_nc_cat=103&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGBXluQwr07H9PvneNH5ygmG5PAxcMjmlsbk8DFwyOaW8LiMOboWIDlmvAuBFVzwOiV4IvPPEW_7assrI-X2qOa&_nc_ohc=caS20MP8ChIAb7EIWIO&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfA9ejhdLKxwjzoEowTXnTxTeDJQLjQPRR3qrb72yxkBHg&oe=6622C04C",
                                    "watermarked_video_sd_url": "",
                                    "watermarked_video_hd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/433234595_1383547219196590_8655084671643865368_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGSZ9fcWX0YhHcPtRfXGkJz-JFXC6DKLnb4kVcLoMoudj7w6Rdj_DQ29vy4F6alJA2vBzRFmjIJtanxA-WN0z37&_nc_ohc=SK5tGkbEy0oAb5-_JY1&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfBqqvqIlNvw1nDUFWGcBElnOWEnip8ARZsV9vjKSIp8qw&oe=6622BC76"
                                }
                            ],
                            "creation_time": 1711296645,
                            "page_id": 107189848084236,
                            "page_name": "Trung Tâm Laptop Hải Phòng",
                            "page_profile_picture_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/434269110_904108448066876_2690975820306820767_n.jpg?stp=dst-jpg_s60x60&_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEIjAtNPMV2S8rW0vPQQq7kvCz96Xqz6iu8LP3perPqK2qe1WAyEwow9bD_aIJCiSp_RaX0IZloRvDNMoD-cwUV&_nc_ohc=WH2ZfTCqMOkAb6msNxp&_nc_oc=AdhFv7nCrC_cDG0hw5LBavRxQw-4l3KfQIoPqwjTjb9TgbLM63VWZfJyYPtPiQztJl0&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfDHxr_dglOsw__cziRQ0CtsLGn_4VSwEw1e4T_gH7iasQ&oe=6622BD14",
                            "page_categories": {
                                "200600219953504": "Shopping"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Trung Tâm Laptop Hải Phòng",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/433142291_1651139268976269_6090089794654941109_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeG1FNo2N2rSHJfebfWXvVex-EbsdxEvNij4Rux3ES82KNCpPaEcGx63hXAP5Ut__Ay7_adF-LfOJdHMd77fOP27&_nc_ohc=rNrb0AtAEmYAb7t_d-Y&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfA_boISjjaMb51NGwtGUQMXNJH6mo3uWbhUwBWQ5vyqpQ&oe=6622D10E",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "🔥  𝐃𝐄𝐋𝐋 𝐋𝐀𝐓𝐈𝐓𝐔𝐃𝐄 𝟓𝟑𝟎𝟎 𝟐-𝐈𝐍-𝟏 -Rẻ đẹp , bền bỉ, đa năng, gập 360 độ cảm ứng<br /> ------------------------------------------<br /> 🔰𝐃𝐞𝐥𝐥 𝐥𝐚𝐭𝐢𝐭𝐮𝐝𝐞 𝟓𝟑𝟎𝟎 𝐢𝟕-𝟖𝟔𝟔𝟓𝐔/ 𝐑𝐚𝐦 𝟏𝟔𝐠𝐛 / 𝐒𝐬𝐝 𝟐𝟓𝟔𝐠𝐛 𝐍𝐯𝐦𝐞 / 𝐌𝐚̀𝐧 𝐟𝐮𝐥𝐥 𝐡𝐝 𝐢𝐩𝐬 / 𝐏𝐢𝐧 𝟑-𝟒𝐡 𝐥𝐢𝐞̂𝐧 𝐭𝐮̣𝐜<br /> 👉 Cấu hình mạnh , mỏng , nhẹ gập 360 độ biến chiếc laptop của bạn thành máy tính bảng rất dễ dàng<br /> 👉 Xử lý được những ứng dụng Văn Phòng, Photoshop, Autocard, Corel, AI, Viết Code lập trình và 1 số game online<br /> ↪️ Ae inbox để được tư vấn ngay nhé !!!<br /> -------------------------------<br /> 𝑯𝒂̉𝒊 𝑷𝒉𝒐̀𝒏𝒈 𝑪𝒐𝒎𝒑𝒖𝒕𝒆𝒓 - 𝑻𝒉𝒆̂́ 𝒈𝒊𝒐̛́𝒊 𝒄𝒐̂𝒏𝒈 𝒏𝒈𝒉𝒆̣̂ 𝒕𝒂̣𝒊 𝑯𝒂̉𝒊 𝑷𝒉𝒐̀𝒏𝒈<br /> 🎁 Tặng ngay Combo Quà tặng or Voucher #200k<br /> ✨ Hỗ trợ trả góp ngay +Đổi mới 15 ngày đầu+Free phần mềm ,vệ sinh<br /> 🏡Địa chỉ : 82-84 Quán Nam, Kênh Dương, Lê Chân, Hải Phòng<br />  ☎ Hotline : 0981.919.595<br /> 🌍 Website : <a href=\"https://l.facebook.com/l.php?u=http%3A%2F%2Fmaytinhhaiphong.com%2F%3Ffbclid%3DIwAR0ZrgxE_q9cxWDCiLXlyrq6YLJRmbIJUfJroSfsEOi2NHnlKHq82NDLxWM&amp;h=AT2qLWKqYikIZ6bwGL-9xgFkRKUYCYhaHhlvAsIbrDhUd7akKwk2hayEWsghfvZ1xJK8GaEd4vDt1eM_P739MrkumYb5rFvx_GWieBiYVF64y9A3pmPrHoczjVTX5mEjj-ngDPj5Zg\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">maytinhhaiphong.com</a>"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Trung Tâm Laptop Hải Phòng",
                            "disclaimer_label": null,
                            "page_like_count": 5502,
                            "page_profile_uri": "https://facebook.com/100091314824136",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712473200,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "297300186733237",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 694041242678550,
                        "currency": "",
                        "endDate": 1713078000,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "107189848084236",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Trung Tâm Laptop Hải Phòng",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120206681696180345",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": null,
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"✅ Tư Vấn Dell inspiron 3520\",\"response\":\"[ NEW 100% ] LAPTOP DELL INSPIRON 3520\\nCPU: I5 - 1235U\\nRAM: 16 GB\\nỔ CỨNG: SSD 512GB\\nĐỒ HOẠ: INTEL IRIS XE GRAPHICS\\nMàn hình : 15'6 FHD ( 120HZ )\\n12,990,000đ\\n- Máy New bảo hành toàn  bộ 12 tháng lỗi 1 đổi 1 trong \\n 30 ngày đầu tiên\"},{\"title\":\"✅ Tư vấn Dell 3511 màn 15'6\"}],\"quick_replies\":[],\"text\":\"Xin chào! Chúng tôi có thể giúp gì cho bạn?\"}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Xin chào! Chúng tôi có thể giúp gì cho bạn?\"}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Xin chào! Chúng tôi có thể giúp gì cho bạn?\"}},\"user_edit\":true,\"surface\":\"visual_editor_new\",\"phone_number\":\"+84778301092\",\"ice_breakers_edited\":true,\"template_id\":\"885980182920834\",\"template_version\":0}",
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "",
                                    "video_sd_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t42.1790-2/388922175_871267664570519_7538821781384003097_n.mp4?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFh7z5NqWRuafOKy3jjaliWS98mUQwaY29L3yZRDBpjbzhDEXCl6agS6IG4C7Gvsm3p6lXhGN2JRWZ_PpyJH-pv&_nc_ohc=nhac2MkUMXwAb7QpsJy&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfCrwQMqUYZTYNLdEvLBDBoj6uIfNfZdATk1jJRQnN4shA&oe=6622B789",
                                    "watermarked_video_sd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/430836219_929546931814638_2036391254873756444_n.jpg?_nc_cat=103&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFvAAkApj-a2zc3XzTt_DKMxr8dTTsob3vGvx1NOyhvex4dxauvzdkfrq2Qg4o3BL8nI48VUrmzEi_ALabAjEKO&_nc_ohc=2yzwbkZOn_QAb7PZUGv&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfB5hAA91seUiVSK0S_XHgvBv6DcVQlXaBNTEI5eQ_Dj8w&oe=6622BC96"
                                }
                            ],
                            "creation_time": 1709346375,
                            "page_id": 107189848084236,
                            "page_name": "Trung Tâm Laptop Hải Phòng",
                            "page_profile_picture_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/430689794_931569728182846_774958951591219005_n.jpg?stp=dst-jpg_s60x60&_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHsBjJ2LkgVcTiZwQlcX9dSlf9m8EnkmCOV_2bwSeSYI0GxHW_eNZziuz1A-IX4kap15G6P4ogs74sxxxr4VW6a&_nc_ohc=CfXY_uHdyS4Ab4ufTF8&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfAnbWvBzdzKKAcRhaBQW5li_m4NJaL_YtLhCmWJO77orw&oe=6622AD54",
                            "page_categories": {
                                "200600219953504": "Shopping"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Trung Tâm Laptop Hải Phòng",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.35426-6/430471270_1483023342628554_6632126995831069603_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHh8wsQOYGp2rMA01YEasdiKh7YUqnjjZIqHthSqeONkhcterGaDLvoiWqMNMVB50HGzm-_AU75EGkR8JwLSPyJ&_nc_ohc=OASJcWqfl0wAb7Q8DeK&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfDkGZV-YcjAfEfhSeSkrNNp178gsmvORX3xze1-uujYYg&oe=6622CC5A",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "Dell inspiron 3520 ( i5 - 1235U / 16G / 512 SSD / màn 15’6 FHD 120hz ) , phù hợp cho sinh viên và dân văn phòng #laptopnew #laptopdell3520 #laptopvanphong #unboxing #laptopdohoa"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Trung Tâm Laptop Hải Phòng",
                            "disclaimer_label": null,
                            "page_like_count": 5502,
                            "page_profile_uri": "https://facebook.com/100091314824136",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712127600,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "1096702818324462",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 953440146389399,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "108625761800188",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Sửa Laptop.Com - Chuyên Sửa Chữa, Nâng Cấp, Laptop,Macbook",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120209798067230454",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "multi_images",
                            "title": null,
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": null,
                            "images": [
                                {
                                    "original_image_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/436934190_3276646025971961_1840942292636112628_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGtM1oqhrkIHs0iLF7-2bwz1KQz2v3ExW7UpDPa_cTFbmov88egxTY3XXt8TX10Yw7Y91JIk0qRWOFvONdmW0wc&_nc_ohc=obIn-b2ZMZcAb4H-GJX&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfDQwTovusli7a4cj37zNt5Mjv0crqV7zToARfvc0Wodhg&oe=6622AA0E",
                                    "resized_image_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/435963302_7695594387169367_2780894679596818859_n.jpg?stp=dst-jpg_s600x600&_nc_cat=103&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGQASweyH_DdiQ0dj_XzZtAK7O0PGTKxiErs7Q8ZMrGIYA5fe4fmPmg76z4QU4ANIOeX0FP48A7exgMtf21KkyP&_nc_ohc=q8Ajt_Y8z-UAb6ew-ts&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfB-zzze5mMkPik5Vs38K0k68aOU5uE1CUTJ_3hjvQNQZA&oe=6622C098",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/436224796_1172850217418327_1029431954593586411_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFfqL_EecVew7SMh2aFAEoCw_xTG0cOeDjD_FMbRw54OH09mvLn2Xe7uRuzW9iYqvyIobWALstLWmYDkX2a8SJ5&_nc_ohc=U9xI34zsgxMAb71Exc8&_nc_oc=Adh3_TKSm2DTvJkxR7cwWObHSGyTPPsSVefn5QUDvRi3YRXLaZudZOHHgkEvUjFceok&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfCgiyy3x4FH2Xw0UAFfvFmic0hOVJBukecm641EqvTMYA&oe=6622C184",
                                    "resized_image_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/436361729_968493321525105_2333293541317213858_n.jpg?stp=dst-jpg_s600x600&_nc_cat=103&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEVboLx9tKXOIWCQbpLKS8W6txl49UY85Pq3GXj1Rjzk-Z0acWOAw8SGNJzp2GFkBhgFOyUGk2W655QwOynSbRJ&_nc_ohc=slE2kdu_9fAAb6TTWGA&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfAc4fG4Mob9Y2qpQBdcVL4iTezlI4kgqjPXUqEREoyQug&oe=6622CDB9",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/436315591_1188028515526693_5375699121914322643_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeElRqnbAcJbWNezutEX7z0k1GwoYGCuu5_UbChgYK67n-VCNClRuMC8Uj3L5YldSMXuxi7B8CtagimtGd1wwgAf&_nc_ohc=DEFlEc-n9AQAb6BP1hF&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfBAIFlQgqnm8_hPPqEOx5FmDQ7yCt9xG2IRhNvEaxo5Yw&oe=6622AADA",
                                    "resized_image_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/436205845_742271218014748_1540036708850944836_n.jpg?stp=dst-jpg_s600x600&_nc_cat=110&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHQrleQc5rX8J_SERgSlDgoAdkUiFT7seUB2RSIVPux5anZh2ISmdhXLncgi6tp2gnotPZrsMp4YGwsp9GcVZtv&_nc_ohc=Qnvd-LEEP7EAb4MiZcc&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfBNkZr26PbfljuczsBcF2AgF53MY35F5hNxKnZVK2teHw&oe=6622AF3E",
                                    "watermarked_resized_image_url": ""
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/436424364_911624070791761_1270722606774625436_n.jpg?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHRwimU7_nJiW2opSLFxhB0BB8nuoWSKhoEHye6hZIqGqqv2tJEUVa7KaL6podo3q7C00h0OUw-4YaEIOgjz_uN&_nc_ohc=clmxLg5yzJEAb7Rf5Df&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfAEt0WNt6uvg-5x7y26d_hjux5sbuYUsYctmXmaitudEA&oe=6622AA99",
                                    "resized_image_url": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.35426-6/436261347_1096429878251393_4256683569924915955_n.jpg?stp=dst-jpg_s600x600&_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGeH6b3bVZEIt23XR87ImeqlNvL_ejXli6U28v96NeWLpXgv3oE8g80ILM2_5daM8SRnQXVKoPwQ44sOqXeFudW&_nc_ohc=AlcGHMvDBeAAb4wAmlc&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfDoxVL9f_-WUGnZKz_r7pATvSO_bWr_dnZLxskam6lf_A&oe=6622D1E2",
                                    "watermarked_resized_image_url": ""
                                }
                            ],
                            "videos": [],
                            "creation_time": 1713077293,
                            "page_id": 108625761800188,
                            "page_name": "Sửa Laptop.Com - Chuyên Sửa Chữa, Nâng Cấp, Laptop,Macbook",
                            "page_profile_picture_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/437056171_1159089748805807_3594752377194435649_n.jpg?stp=dst-jpg_s60x60&_nc_cat=110&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeG86CORmhkhPjZr3i-92iCMjwl8d56NfbqPCXx3no19uuaxU7H5V6CI0copN5uwaGFnbt2JvjL6c_mkL4WcyKeA&_nc_ohc=mzQNplkO2R0Ab6kCtV8&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfCGcXwq4zICJidRHDHa_v5HkJpcfV3EfbZ43BxquyYsSg&oe=6622C535",
                            "page_categories": {
                                "108472109230615": "Computer Service"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Sửa Laptop.Com - Chuyên Sửa Ch",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.35426-6/436311091_780405567069642_6132326755126397334_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGiz92ckvyu5RrINDVTg7d_SW14I1QzQRtJbXgjVDNBG0yzcBu0GoRG9y67ISsANy6-PuvsJjxu2ZHvyalRbmKq&_nc_ohc=9JvGwjSw5lwAb7_OCdJ&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfBMYv7TzSw4k0jsP_pJHssv5rxIxOdBrxzJ-AWy64QH_g&oe=6622B6CE",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "⚡️ Giải pháp toàn diện cho Laptop của bạn tại <a href=\"https://l.facebook.com/l.php?u=http%3A%2F%2FSualaptop.com%2F%3Ffbclid%3DIwAR3hkIMGstcK24Fm4KQiK5NMkuRl0uKVHiH8TqI3XimZl-gd96QsrO2zDlU&amp;h=AT2otLI2DkBsrHZ2OdVWlQqFGgtGPbt_wG9nS-VZKu8HcMYQTqTHnEyLd7kbR0VnEKi5v90E3J2Do6AuTrNOC2PW-caVpIokiZVjoAR1779XoYgE3Ni1cwGxnFLQzOTM9h-ZDSsm5w\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">Sualaptop.com</a><br /> 💥 Sửa chữa phần cứng, Nâng cấp, Thay thế linh kiện, Vệ sinh - Bảo dưỡng máy,....<br /> ☄️ Thời gian thực hiện nhanh chóng, Khách có thể trực tiếp xem, nhận máy ngay<br /> 🛡 Chế độ bảo hành đầy đủ, Hậu mãi dài hạn<br /> 🎉 Ưu đãi đặc biệt cho Sinh viên và Khách hàng cũ<br /> &gt;&gt; Liên hệ ngay để được hỗ trợ tư vấn miễn phí nhé!!<br /> <br />  👉 HỆ THỐNG SỬA <a href=\"https://l.facebook.com/l.php?u=http%3A%2F%2FLAPTOP.COM%2F%3Ffbclid%3DIwAR3_WqIRo0-3yOhZmdkgt5D4xjloKP9uTrZtcSlyYkVIP8J5KIYfPJFm5Ic&amp;h=AT36GqHWrsFJl4FHs0pWGfqF95tXDN9UWtjtntLlMn0sd1ZN1LFQEmWrsEfsEx3CXtqkYTnkajW-HKponmZ0Uy4-z0rbrnfHM9NgLQ_bxHJnQAmXwtLWItnl5wvh3i77k3TXO8kmRA\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">LAPTOP.COM</a> <br /> 🔗 Website : <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fsualaptop.com%2F%3Ffbclid%3DIwAR0hJpEZk3z0r4tqDexOdpXPAzQDXCh0wqy8rWXn2IdLV4k9M495Rzu7qP8&amp;h=AT062eg7SEUh9JXAXsnp1SA6YSzrwIdLrqssF3Cfu1rVvDA9jPgmn2xQLCAsgLKxjLHIvlLz3VkBKTtyWNJk19MqoIZ0jVLjq7VchE2UAG2gbK3l23pK37-9W0tQCFgcoOQfYXdatg\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://sualaptop.com/</a><br /> 📞 Hotline: 0934.567.628<br /> <br /> ✅ Địa chỉ 1: 861 Lạc Long Quân Phường 8 Quận Tân Bình<br /> ☎️CN Tân Bình : 0934.567.628<br /> <br /> ✅ Địa chỉ 2: 22 Võ Trường Toản, P.2, Q.Bình Thạnh, TPHCM<br /> ☎️CN Bình Thạnh : 0909.668.027<br /> <br /> ✅ Địa chỉ 3: 291 Tân Sơn Nhì, P. Tân Sơn Nhì, Q. Tân Phú, Tp. HCM<br /> ☎️CN Tân Phú : 0939.631.268<br /> <br /> #sualaptop <br /> #sualaptopquantanbinh    <br /> #sualaptopganday  <br /> #sualaptopgiare  <br /> #sualaptoptphcm  <br /> #sualaptoptanphu  <br /> #sualaptopquanbinhthanh  <br /> #sualaptoplayngay"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Sửa Laptop.Com - Chuyên Sửa Chữa, Nâng Cấp, Laptop,Macbook",
                            "disclaimer_label": null,
                            "page_like_count": 4739,
                            "page_profile_uri": "https://facebook.com/sualaptopcom",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1713078000,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "1110100190211967",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 308601655058818,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "108625761800188",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Sửa Laptop.Com - Chuyên Sửa Chữa, Nâng Cấp, Laptop,Macbook",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120209803866610454",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": null,
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Tôi cần tư vấn dịch vụ sửa chữa Laptop.\",\"response\":\"Chào {{user_full_name}} . Laptop A/c đang gặp tình trạng lỗi như thế nào vui lòng cho shop biết shop hỗ trợ tư vấn cho mình ạ.\"},{\"title\":\"Tôi cần tư vấn dịch vụ sửa chữa Macbook.\",\"response\":\"Chào {{user_full_name}} . Macbook A/c đang gặp tình trạng lỗi như thế nào vui lòng cho shop biết shop hỗ trợ tư vấn cho mình ạ.\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting\":false}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting\":false}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\",\"is_eligible_for_customized_greeting\":false}},\"user_edit\":true,\"surface\":\"visual_editor_new\",\"ice_breakers_edited\":true,\"template_id\":\"298220843307083\"}",
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "https://scontent.fsgn2-5.fna.fbcdn.net/v/t42.1790-2/10000000_1110100206878632_4599877657429238899_n.?_nc_cat=104&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFbyqwHzRvWRLNYlyXr5L0TbTxRE5ccQr5tPFETlxxCvgt9_duMUwMpodhgf1Ex3yQkUz9NcihoTWw_aju5RIkR&_nc_ohc=QlVdNMpBSrIAb78dnMj&_nc_ht=scontent.fsgn2-5.fna&oh=00_AfCXJrkhyH0a1jMZkDZfOt8qFGlrbiRJySUf_Fp3dVot_w&oe=6622DBF8",
                                    "video_sd_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t42.1790-2/370813077_1497799580990448_3072851012784657086_n.mp4?_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFkLcG-dQwT6zniAY8r5hb4zMYykEtnmWDMxjKQS2eZYMRXv8lgX_iMzeAXocicv2gFityZ4fCwdjeFv_67xGSG&_nc_ohc=97K1COSPIVEAb4Vxnj7&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfDm1jEt5qnedTIoNbVRme9WEpNtSGRBflyiuYUmxp20dg&oe=6622BB61",
                                    "watermarked_video_sd_url": "",
                                    "watermarked_video_hd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/437044378_1450416559194074_5985077730161907152_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGFW66FbXdYzrR5EAqpaR09AdPrSMoTR2IB0-tIyhNHYl9NjUupRStdbgKToYIMAw8xkVQpcP_VBqG29Qy8rg-3&_nc_ohc=9XXg3vvLx24Ab55pUWK&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfB5_AJM5wLGtEsDT1lysLo2-rfvWyTjRyTV9otGfxl2nw&oe=6622DBCE"
                                }
                            ],
                            "creation_time": 1713090814,
                            "page_id": 108625761800188,
                            "page_name": "Sửa Laptop.Com - Chuyên Sửa Chữa, Nâng Cấp, Laptop,Macbook",
                            "page_profile_picture_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/437054600_727837376186378_8447261419401345662_n.jpg?stp=dst-jpg_s60x60&_nc_cat=106&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEZdYfLLaGX0-PozHMJ70rhB_4-hnbPhtsH_j6Gds-G28QSVaVQz674HY1jv1NnVuBOeB3gE3G1kTQlMq4LSnIX&_nc_ohc=WyB7yCMof3sAb7tuYpC&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfDaKjcE72d1LKprmG8BiKcmZr9kp8S5XDXkeu29QTdrWg&oe=6622C542",
                            "page_categories": {
                                "108472109230615": "Computer Service"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Sửa Laptop.Com - Chuyên Sửa Ch",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/437158908_1619416495498380_1602531656596110416_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFihBp3i5Xhaah5v3BFA-t0oTE6ZvmuT0GhMTpm-a5PQcwosAd0QVwvJBlgznMeKZQLOgkmK60p6I85flDFnyCi&_nc_ohc=p78MLAMhv_UAb4YKeXn&_nc_oc=Adgag8hCJAbmZ1L7U44oIGE5JEcV-0iAUOOPpNH4sWcvowB55uiwfds0cHzeAmsRUBA&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfDJ_vfBboQeGC1Q-FZLLFLnRnZRT1oqiI1k51anEzEwQg&oe=6622CFC5",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "⭕️Sửa Chữa, Nâng Cấp #LAPTOP - #MACBOOK - Lấy Liền Giá Rẻ, Xem Trực Tiếp⭕️<br /> 💥Ưu Đãi Giảm Giá Lên Đến 30%<br /> 🌐Link Xem Chi Tiết : <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fsualaptop.com%2F%3Ffbclid%3DIwAR0g9xmNXgtnPB1SwnzF9XLmQhIuSBwRuNhnbTDBi5OAy92rTA3jYk8dZuk&amp;h=AT0R1WvQQ-IygyFtv08c2dxO8HF6nDXNoX4jZtCx34xl1en03Q4bLilWGIUi2y-1h6u8g_ALDZ-ukYTztGyTvUcJ7v8aGfBGhkGUP0UKy1zjevS3n7aZ9EFdbYYjdEfM-XIz9OP1Dw\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://sualaptop.com/</a><br /> --------------------------------------------<br /> 💢CAM KẾT DỊCH VỤ<br /> ✔️Tư vấn, kiểm tra báo bệnh miễn phí<br /> ✔️Xem trực tiếp quá trình sửa chữa. bảo hành lâu dài nhanh gọn<br /> ✔️Nhiều chi nhánh, kỹ thuật viên nhiều năm kinh nghiệm<br /> ✔️Báo đúng bệnh, đúng giá, minh bạch không hài lòng hoàn tiền<br /> -------------------------------------------<br /> 💢THÔNG TIN LIÊN HỆ<br /> 🏢 Địa chỉ 1: 861 Lạc Long Quân Phường 8 Quận Tân Bình<br /> 🏢 Địa chỉ 2: 22 Võ Trường Toản, P.2, Q.Bình Thạnh, TPHCM<br /> 🏢 Địa chỉ 3: 291 Tân Sơn Nhì, P. Tân Sơn Nhì, Q. Tân Phú, Tp. HCM<br /> 🌐 Website : <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fsualaptop.com%2F%3Ffbclid%3DIwAR3zfbAz2Uq2rPFgNLPzS-LCr-YXdkMPbqE8F2o0e9lQxXex4DyGWo6p2hs&amp;h=AT1yR_9L9krvK9qz2fRR9_eeb8VHdbnrL-6an8msVR2LeLFBPbu0ETKCM2egF9HMAwk6l_h_BqNKrxSbeIn2ckEjjcQN0DpKYx6y-nzIW2NN9O1nzSwspbyuCP6fN68oebRCcDl19g\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://sualaptop.com/</a><br /> ☎ Hotline: 0934.567.628<br /> ☎ CN Tân Bình : 0934.567.628<br /> ☎ CN Tân Phú : 0939.631.268<br /> ☎ CN Bình Thạnh : 0909.668.027"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Sửa Laptop.Com - Chuyên Sửa Chữa, Nâng Cấp, Laptop,Macbook",
                            "disclaimer_label": null,
                            "page_like_count": 4739,
                            "page_profile_uri": "https://facebook.com/sualaptopcom",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1713078000,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "1648857282521016",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 1379805419565283,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "431174533597859",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Thu Mua Laptop Cũ Giá Cao - Kỹ Nghệ Laptop Cần Thơ",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": 6560672821104,
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": "fb.com",
                            "cta_text": "Truy cập trang cá nhân",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "image",
                            "title": "www.fb.com",
                            "link_description": null,
                            "link_url": "http://www.fb.com/100057676890954",
                            "page_welcome_message": null,
                            "images": [
                                {
                                    "original_image_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.35426-6/435890498_779109870826811_8677551029400108478_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHxhUe2lJ9KFbfi72GNQ3EG2PC1jF0IIE3Y8LWMXQggTcKUTmlRXC10tkE0BfuqrOgU2MgW_DlEzFJ3-AMi6Z1t&_nc_ohc=XIqrmm0H374Ab4D_p-0&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDFPIROcBkuY_xTZaYuYXze8bsyKI5SLOCMCko2yydt3Q&oe=6622D614",
                                    "resized_image_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/435716264_396770849786515_831145394033704820_n.jpg?stp=dst-jpg_s600x600&_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEHAcSFth1_8MIghLlZIJ5IhHY0XeNne1-EdjRd42d7X7OW-gA52OV1PXkZ4GP8L5W9ipSDCpoSA4AeatC91z5M&_nc_ohc=tHDp7LEuJUAAb6-phQX&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfBcIGsIQZya32-4SgausFzOVA23o_aV3CXjFkFvkeg5fg&oe=6622CAFD",
                                    "watermarked_resized_image_url": "",
                                    "image_crops": {}
                                }
                            ],
                            "videos": [],
                            "creation_time": 1712979174,
                            "page_id": 431174533597859,
                            "page_name": "Thu Mua Laptop Cũ Giá Cao - Kỹ Nghệ Laptop Cần Thơ",
                            "page_profile_picture_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/435700075_962323335401618_1908702678419626166_n.jpg?stp=dst-jpg_s60x60&_nc_cat=106&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHmit-T8PSGKRh1m58c3YBFhKaHw0SijvWEpofDRKKO9YEYcTuX9GJFQzDXcbUnx2jWGFzhrq_nXQhvICNM2wih&_nc_ohc=gtczyz1SmPUAb40CVzy&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfAdjtrv4k7bOUefXJlD_tSXViIpf05UYFFY53q2xh6vpQ&oe=6622B6C7",
                            "page_categories": {
                                "2255": "Computer Company"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Thu Mua Laptop Cũ Giá Cao - Kỹ",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/435694598_1344535529717948_4978113335502314722_n.jpg?_nc_cat=103&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFuMINnlsxxoov0nTaSRTaKjflcLoQgHHKN-VwuhCAccptN_-ItxYig72kCPrxG762EBUFIpny3coVnR4CfDppJ&_nc_ohc=J3Q_i-3d4YoAb6zA13R&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfAcGajnc3hdoRl6RBh8O8pGqZKTqCPH75agOWavIWD2cA&oe=6622C55F",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "Thu Mua Laptop- Gaming-Macbook giá cao tại Cần Thơ"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Thu Mua Laptop Cũ Giá Cao - Kỹ Nghệ Laptop Cần Thơ",
                            "disclaimer_label": null,
                            "page_like_count": 553,
                            "page_profile_uri": "https://facebook.com/KyNgheLaptop",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "VISIT_PROFILE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712905200,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "1590313868389207",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 994979668171030,
                        "currency": "",
                        "endDate": 1713078000,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "102007079344701",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Azskin.vn - Skin Laptop, Điện Thoại, Máy Ảnh Theo Yêu Cầu",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120210289268800631",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": "Dán skin laptop in hình theo yêu cầu | AZSKIN",
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Dán skin laptop giá bao nhiêu?\"},{\"title\":\"Tôi muốn dán skin laptop in hình theo yêu cầu.\"},{\"title\":\"Địa chỉ cửa hàng AZSKIN ở đâu?\"}],\"quick_replies\":[],\"text\":\"Cảm ơn anh/chị đã quan tâm dịch vụ dán skin Laptop tại AZSKIN. Nhân viên tư vấn sẽ hỗ trợ mình trong ít phút ạ\"},\"in_thread_multiphoto_carousel\":{\"is_enabled\":false,\"button\":{\"action_prefill\":\"Mặt hàng này còn không?\",\"response\":\"Cảm ơn bạn đã quan tâm. Chúng tôi sẽ liên hệ lại với bạn để thông báo về tình trạng hàng của mặt hàng này.\",\"title\":\"Hỏi tình trạng hàng\",\"type\":\"availability\"}}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Cảm ơn anh/chị đã quan tâm dịch vụ dán skin Laptop tại AZSKIN. Nhân viên tư vấn sẽ hỗ trợ mình trong ít phút ạ\"}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Cảm ơn anh/chị đã quan tâm dịch vụ dán skin Laptop tại AZSKIN. Nhân viên tư vấn sẽ hỗ trợ mình trong ít phút ạ\"}},\"user_edit\":true,\"surface\":\"visual_editor_new\",\"template_id\":\"1353215772113287\"}",
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t42.1790-2/10000000_1590313931722534_3008045606699017220_n.?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEQEfp7xjWwdnOFILd6OlEAelRXlEZyGwJ6VFeURnIbAoxnFnAYDncD2qMQ5N_AyEA-VurfBturPc7yqkzppnXK&_nc_ohc=_MyQgfdO0JQAb7O3B2M&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfD1yogRrWjZfBAIgjzRocCRX2-jpSsCcqQ7RE3KACdczA&oe=6622C979",
                                    "video_sd_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t42.1790-2/435222827_25505209469070193_2137850316120888954_n.mp4?_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHRGj0A4q7iCNufy1YcnwX-5F_BCnYnvLDkX8EKdie8sA8P2-ieBe2lopfW0pcqPiwOfZxZRLEsTZ0WbxlO9I8p&_nc_ohc=Nal9yaLKhYkAb70RCoP&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfA_w4U6eqzl7ktxQTb6i99jeg40_eJT3bglq9Zs49F-Cg&oe=6622C887",
                                    "watermarked_video_sd_url": "",
                                    "watermarked_video_hd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.35426-6/434424231_1423988494920326_3563049208397907359_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFkkv7WAdS0JJuVd4LUED6e5VERRHb377vlURFEdvfvu-IuxZfMXdlstw5uVQBTiq-cKXTvMVouIDw3oD5h2tht&_nc_ohc=j2NZbOGSJ8cAb4CnMSw&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfCeJrPa6mcJZKJi7Qvi-kxwzLNy4bhSQ0b3KStclLtzaA&oe=6622D30A"
                                }
                            ],
                            "creation_time": 1712131186,
                            "page_id": 102007079344701,
                            "page_name": "Azskin.vn - Skin Laptop, Điện Thoại, Máy Ảnh Theo Yêu Cầu",
                            "page_profile_picture_url": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.35426-6/434042169_1080054656431212_2768988181436208710_n.jpg?stp=dst-jpg_s60x60&_nc_cat=103&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeH6e0VDBfwpnCoD8zZWhYoygqZOdM6Q7smCpk50zpDuyQIQJmlBpdJXzb5UD6hfIRU3whgLYdByYZXHUhxIV4IJ&_nc_ohc=wRjWwo8yx-0Ab459kDm&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfCdDEfqr5TnTxYaex2UHvVYbu50vJfUisV_boA9E7_xNw&oe=6622AA1C",
                            "page_categories": {
                                "1615": "Designer"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Azskin.vn - Skin Laptop, Điện",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.35426-6/433997805_971503357713246_8325619730339436914_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGyD7Urchwf9rWr6lYqVwr2hn81ZlyElNWGfzVmXISU1WEf9KYlfrdqocM8IcGqJUy7L4sdhPgjDPkn-gJuHSB6&_nc_ohc=RCp0qfgygb8Ab63FFMU&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDGprAS7bMm6Q7tDyiD4JcbKTkT29PNIIQLiX3Pi_O25g&oe=6622CDDA",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "Dán skin laptop siêu nét với công nghệ in mới nhất hiện nay 😍 In hình theo yêu cầu cho mọi dòng máy 🎉<br /> <br /> ▪️  Bảo vệ laptop khỏi trầy xước, bám bẩn<br /> ▪️  Công nghệ in sắc nét từng chi tiết<br /> ▪️  Bám dính chắc chắn, không để lại keo khi gỡ<br /> <br /> Hỗ trợ dán cho khách hàng ghé trực tiếp hệ thống cửa hàng của Azskin trên toàn quốc<br /> ---------------------------------<br /> ☎️ Hotline: 0948.911.111 - 0585.188.188<br /> ⏰ Time: 8h30 - 21h00 (Thứ 2 đến Chủ nhật)<br /> 🏤 Azskin Hà Nội:<br />      ▪️  122A Ngọc Hà, Ba Đình, HN<br />      ▪️  76 Ngõ 259 Phố Vọng, Hai Bà Trưng, HN<br />      ▪️  3 Ngõ 31 Dịch Vọng, Cầu Giấy, HN<br />      ▪️  2 Ngõ 18 Nguyễn Khuyến, Hà Đông, HN<br />      ▪️  46 Hồng Tiến, P. Bồ Đề, Long Biên, HN<br />      ▪️  5 Phố Nguyễn Mậu Tài, Trâu Quỳ, Gia Lâm, HN<br />      ▪️  148 Cao Lỗ, Đông Anh, Hà Nội"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Azskin.vn - Skin Laptop, Điện Thoại, Máy Ảnh Theo Yêu Cầu",
                            "disclaimer_label": null,
                            "page_like_count": 1184,
                            "page_profile_uri": "https://facebook.com/azskin.laptop",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712127600,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "787954509557148",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 6,
                        "collationID": 1387972795189091,
                        "currency": "",
                        "endDate": 1713078000,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "1743192135981478",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "MrLaptop.vn",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120208294377630443",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "image",
                            "title": "💥SỬA LAPTOP GIẢM ĐẾN 50%",
                            "link_description": "Hơn +950.000 Khách hàng đã nhắn tin",
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Địa chỉ của bạn ở đâu?\",\"response\":\"\"},{\"title\":\"Tư vấn sửa laptop\"},{\"title\":\"Báo giá sửa laptop\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"user_edit\":true,\"surface\":\"visual_editor_new\",\"ice_breakers_edited\":true,\"template_id\":\"351556517311891\"}",
                            "images": [
                                {
                                    "original_image_url": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.35426-6/433104836_1513102186297443_371383041104236458_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGzfeQev1MkEKvzXwIusGsN0IENphtwSGPQgQ2mG3BIY2jDp7PPdkh4XWf2izp6wlapjB-EVhT0nC5WfFjeE2Sj&_nc_ohc=1p9YRiypwVQAb6ZjuFn&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfBUY96AwT4lIXuKH7yqCNjXYgJaVZ1xxjj-Pzq8PhK_ag&oe=6622B207",
                                    "resized_image_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/433139917_880602107196683_1116506191046180442_n.jpg?stp=dst-jpg_s600x600&_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFQVfuWufBFgRWOnFIFVjU1Mc0H6R-932ExzQfpH73fYVB8rmIeVD5Bl44Kdn754hsV8v-JhttUdtFoSBf6qHjS&_nc_ohc=7_jhhJtNUWgAb7_Qmdk&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfC2tGAd_Hd4Qs2rewd309egNwycQ5hR2RzC7ctck29mXQ&oe=6622AAB2",
                                    "watermarked_resized_image_url": "",
                                    "image_crops": {}
                                }
                            ],
                            "videos": [],
                            "creation_time": 1711554525,
                            "page_id": 1743192135981478,
                            "page_name": "MrLaptop.vn",
                            "page_profile_picture_url": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.35426-6/434293266_1962626297472535_2644820402052483544_n.jpg?stp=dst-jpg_s60x60&_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHxG4mhMT-mb1FSmpg_kqyRn2GNbWOGzQ-fYY1tY4bND2VOc5LyLXy95XBMfEB59Enznx7Us0cDrNdAtM2itwCW&_nc_ohc=87HeqG5nUjcAb5_HA-N&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfBWcgObYrG3rcbABmFmjU1khX38J6nDCVNBAwdlsP91Jg&oe=6622CFD2",
                            "page_categories": {
                                "199512783398620": "Electronics"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "MrLaptop.vn",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/433060037_1260682638225808_3787351682230697281_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHGs0hpnIbuZ7U9KWUOKhRjbzNnYR_G6AFvM2dhH8boAUQ5mRzfo9EHoy1tpKqox0DUop1a-JeJdGMB65Hk3Uzy&_nc_ohc=lu6Zicydo6sAb42Ih8j&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfCdUurPNSYcsKZm5mwpkzaNIC6LDq1VQMcVHQedEcfl2Q&oe=6622B7CD",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "#Sửa_Laptop, Nâng Cấp 𝐋𝐀𝐏𝐓𝐎𝐏 - 𝐌𝐀𝐂𝐁𝐎𝐎𝐊<br /> 👉Khai Trương Chi Nhánh Mới 𝖦𝗂ảm 30-50%<br /> <br /> 💻Ѕửа mất nɡuồn сһἰ từ 300.000đ<br /> 💻Ѕửа màn һὶnһ сһἰ từ 250.000đ<br /> 💻Nânɡ сấр rаm сһἰ từ 150.000đ<br /> 💻Тһау bàn рһίm сһἰ từ 290.0000đ<br /> 💻Тһау р𝗂n ⅼарtор сһἰ từ 390.000đ<br /> <br /> Bảnɡ ɡ𝗂á: <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fmrlaptop.vn%2Fbang-gia-dich-vu-sua-laptop-lay-lien%2F%3Ffbclid%3DIwAR2zANzp2BdjR3wBaT5drHDQVmfJL1-xmoKlKXlmhVUvgq84tyC2QY5d2lA&amp;h=AT3BSmgHEQHl2dKyvtRSCWdwwPupAbfobkAw0d17cfSgooPp0u9L1L3mKDcJlt-2T5lmRG9WnClcUeemKS5WG-lt_Bp7BxkczVg5W3eOIbBrY_omvbYvLjO1KYADlt1pULxiGrF__g\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://mrlaptop.vn/bang-gia-dich-vu-sua-laptop-lay-lien/</a><br /> <br /> 𝐇𝐄̣̂ 𝐓𝐇𝐎̂́𝐍𝐆 𝐒𝐔̛̉𝐀 𝐂𝐇𝐔̛̃𝐀 𝐋𝐀𝐏𝐓𝐎𝐏 - 𝐌𝐀𝐂𝐁𝐎𝐎𝐊 𝐔𝐘 𝐓𝐈́𝐍:<br /> <br /> ✔ СN1: 127 đườnɡ 3/2, Рһườnɡ 11, Ԛuận 10<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: 9һ00-17һ00 - 𝖧оtⅼ𝗂nе: 0931.640.640<br /> <br /> ✔ СN2: 514 Сáсһ Mạnɡ Тһánɡ 8, Р11, Ԛuận 3<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0968.450.450<br /> <br /> ✔ СN3: 167А Đàо 𝖣uу Аnһ, Р9, Рһú Nһuận<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0931.590.590<br /> <br /> ✔ СN4: 203А Ⅼê Ԛuаnɡ Địnһ, Р7, Bὶnһ Тһạnһ<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0934.032.032<br /> <br /> ✔ СN5: 1068B Âu Сơ, Р14, Тân Bὶnһ<br /> (Сửа һànɡ màu đỏ 1068 сó 3 сăn ⅼ𝗂ền kề)<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0936.590.590<br /> <br /> ✔ СN6: 457 Ⅼê 𝖵ăn Тһọ, Р9, 𝖦ò 𝖵ấр<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0966.430.430<br /> <br /> ✔ СN7: 678 Kһа 𝖵ạn Сân, Р. Ⅼ𝗂nһ Đônɡ, Тһủ Đứс<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0962.710.710<br /> <br /> ✔ СN8: 46 𝖣ươnɡ Đὶnһ 𝖧ộ𝗂, Рһướс Ⅼоnɡ B, Тһủ Đứс (Ԛuận 9 сũ)<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0964.260.260<br /> <br /> ✔ СN9: 1020 𝖧ậu 𝖦𝗂аnɡ, Р12, Ԛuận 6<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0923.450.450<br /> <br /> #sửa_laptop  #sửa_macbook #mrlaptop"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "MrLaptop.vn",
                            "disclaimer_label": null,
                            "page_like_count": 5818,
                            "page_profile_uri": "https://facebook.com/mrlaptop.vn",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1712473200,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    },
                    {
                        "adid": "0",
                        "adArchiveID": "1115721596291952",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": null,
                        "collationID": 1387972795189091,
                        "currency": "",
                        "endDate": 1713164400,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "1743192135981478",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "MrLaptop.vn",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120208294377630443",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "image",
                            "title": "💥SỬA LAPTOP GIẢM ĐẾN 50%",
                            "link_description": "Hơn +950.000 Khách hàng đã nhắn tin",
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Địa chỉ của bạn ở đâu?\",\"response\":\"\"},{\"title\":\"Tư vấn sửa laptop\"},{\"title\":\"Báo giá sửa laptop\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"user_edit\":true,\"surface\":\"visual_editor_new\",\"ice_breakers_edited\":true,\"template_id\":\"351556517311891\"}",
                            "images": [
                                {
                                    "original_image_url": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.35426-6/433104836_1513102186297443_371383041104236458_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGzfeQev1MkEKvzXwIusGsN0IENphtwSGPQgQ2mG3BIY2jDp7PPdkh4XWf2izp6wlapjB-EVhT0nC5WfFjeE2Sj&_nc_ohc=1p9YRiypwVQAb6ZjuFn&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfBUY96AwT4lIXuKH7yqCNjXYgJaVZ1xxjj-Pzq8PhK_ag&oe=6622B207",
                                    "resized_image_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/433139917_880602107196683_1116506191046180442_n.jpg?stp=dst-jpg_s600x600&_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFQVfuWufBFgRWOnFIFVjU1Mc0H6R-932ExzQfpH73fYVB8rmIeVD5Bl44Kdn754hsV8v-JhttUdtFoSBf6qHjS&_nc_ohc=7_jhhJtNUWgAb7_Qmdk&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfC2tGAd_Hd4Qs2rewd309egNwycQ5hR2RzC7ctck29mXQ&oe=6622AAB2",
                                    "watermarked_resized_image_url": "",
                                    "image_crops": {}
                                }
                            ],
                            "videos": [],
                            "creation_time": 1711554525,
                            "page_id": 1743192135981478,
                            "page_name": "MrLaptop.vn",
                            "page_profile_picture_url": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.35426-6/434293266_1962626297472535_2644820402052483544_n.jpg?stp=dst-jpg_s60x60&_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHxG4mhMT-mb1FSmpg_kqyRn2GNbWOGzQ-fYY1tY4bND2VOc5LyLXy95XBMfEB59Enznx7Us0cDrNdAtM2itwCW&_nc_ohc=87HeqG5nUjcAb5_HA-N&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfBWcgObYrG3rcbABmFmjU1khX38J6nDCVNBAwdlsP91Jg&oe=6622CFD2",
                            "page_categories": {
                                "199512783398620": "Electronics"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "MrLaptop.vn",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/433060037_1260682638225808_3787351682230697281_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHGs0hpnIbuZ7U9KWUOKhRjbzNnYR_G6AFvM2dhH8boAUQ5mRzfo9EHoy1tpKqox0DUop1a-JeJdGMB65Hk3Uzy&_nc_ohc=lu6Zicydo6sAb42Ih8j&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfCdUurPNSYcsKZm5mwpkzaNIC6LDq1VQMcVHQedEcfl2Q&oe=6622B7CD",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "#Sửa_Laptop, Nâng Cấp 𝐋𝐀𝐏𝐓𝐎𝐏 - 𝐌𝐀𝐂𝐁𝐎𝐎𝐊<br /> 👉Khai Trương Chi Nhánh Mới 𝖦𝗂ảm 30-50%<br /> <br /> 💻Ѕửа mất nɡuồn сһἰ từ 300.000đ<br /> 💻Ѕửа màn һὶnһ сһἰ từ 250.000đ<br /> 💻Nânɡ сấр rаm сһἰ từ 150.000đ<br /> 💻Тһау bàn рһίm сһἰ từ 290.0000đ<br /> 💻Тһау р𝗂n ⅼарtор сһἰ từ 390.000đ<br /> <br /> Bảnɡ ɡ𝗂á: <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fmrlaptop.vn%2Fbang-gia-dich-vu-sua-laptop-lay-lien%2F%3Ffbclid%3DIwAR0f85zZME_PLQf8uIwj1lzo6QXL6zTp-vmQdcRLIBXrsBQCrIFQt36oL2A&amp;h=AT1Ng2aFJ0_qsylQZ-qzEK52dA2N3-xhVq3r7p2kk_BE605UNuF_f8C-ADEzK5jSyuOuI3DYy_2lKajQf8ozvFugZ6uzd7a_OolYYdB3Z5EEWv0VZd9uzxpAnsrxZZJKUHgVuXmmnA\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://mrlaptop.vn/bang-gia-dich-vu-sua-laptop-lay-lien/</a><br /> <br /> 𝐇𝐄̣̂ 𝐓𝐇𝐎̂́𝐍𝐆 𝐒𝐔̛̉𝐀 𝐂𝐇𝐔̛̃𝐀 𝐋𝐀𝐏𝐓𝐎𝐏 - 𝐌𝐀𝐂𝐁𝐎𝐎𝐊 𝐔𝐘 𝐓𝐈́𝐍:<br /> <br /> ✔ СN1: 127 đườnɡ 3/2, Рһườnɡ 11, Ԛuận 10<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: 9һ00-17һ00 - 𝖧оtⅼ𝗂nе: 0931.640.640<br /> <br /> ✔ СN2: 514 Сáсһ Mạnɡ Тһánɡ 8, Р11, Ԛuận 3<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0968.450.450<br /> <br /> ✔ СN3: 167А Đàо 𝖣uу Аnһ, Р9, Рһú Nһuận<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0931.590.590<br /> <br /> ✔ СN4: 203А Ⅼê Ԛuаnɡ Địnһ, Р7, Bὶnһ Тһạnһ<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0934.032.032<br /> <br /> ✔ СN5: 1068B Âu Сơ, Р14, Тân Bὶnһ<br /> (Сửа һànɡ màu đỏ 1068 сó 3 сăn ⅼ𝗂ền kề)<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0936.590.590<br /> <br /> ✔ СN6: 457 Ⅼê 𝖵ăn Тһọ, Р9, 𝖦ò 𝖵ấр<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0966.430.430<br /> <br /> ✔ СN7: 678 Kһа 𝖵ạn Сân, Р. Ⅼ𝗂nһ Đônɡ, Тһủ Đứс<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0962.710.710<br /> <br /> ✔ СN8: 46 𝖣ươnɡ Đὶnһ 𝖧ộ𝗂, Рһướс Ⅼоnɡ B, Тһủ Đứс (Ԛuận 9 сũ)<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0964.260.260<br /> <br /> ✔ СN9: 1020 𝖧ậu 𝖦𝗂аnɡ, Р12, Ԛuận 6<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0923.450.450<br /> <br /> #sửa_laptop  #sửa_macbook #mrlaptop"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "MrLaptop.vn",
                            "disclaimer_label": null,
                            "page_like_count": 5818,
                            "page_profile_uri": "https://facebook.com/mrlaptop.vn",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1711954800,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    },
                    {
                        "adid": "0",
                        "adArchiveID": "736905655244278",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": null,
                        "collationID": 1387972795189091,
                        "currency": "",
                        "endDate": 1713078000,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "1743192135981478",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "MrLaptop.vn",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120208294377630443",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "image",
                            "title": "💥SỬA LAPTOP GIẢM ĐẾN 50%",
                            "link_description": "Hơn +950.000 Khách hàng đã nhắn tin",
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Địa chỉ của bạn ở đâu?\",\"response\":\"\"},{\"title\":\"Tư vấn sửa laptop\"},{\"title\":\"Báo giá sửa laptop\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"user_edit\":true,\"surface\":\"visual_editor_new\",\"ice_breakers_edited\":true,\"template_id\":\"351556517311891\"}",
                            "images": [
                                {
                                    "original_image_url": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.35426-6/433104836_1513102186297443_371383041104236458_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGzfeQev1MkEKvzXwIusGsN0IENphtwSGPQgQ2mG3BIY2jDp7PPdkh4XWf2izp6wlapjB-EVhT0nC5WfFjeE2Sj&_nc_ohc=1p9YRiypwVQAb6ZjuFn&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfBUY96AwT4lIXuKH7yqCNjXYgJaVZ1xxjj-Pzq8PhK_ag&oe=6622B207",
                                    "resized_image_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/433139917_880602107196683_1116506191046180442_n.jpg?stp=dst-jpg_s600x600&_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFQVfuWufBFgRWOnFIFVjU1Mc0H6R-932ExzQfpH73fYVB8rmIeVD5Bl44Kdn754hsV8v-JhttUdtFoSBf6qHjS&_nc_ohc=7_jhhJtNUWgAb7_Qmdk&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfC2tGAd_Hd4Qs2rewd309egNwycQ5hR2RzC7ctck29mXQ&oe=6622AAB2",
                                    "watermarked_resized_image_url": "",
                                    "image_crops": {}
                                }
                            ],
                            "videos": [],
                            "creation_time": 1711554525,
                            "page_id": 1743192135981478,
                            "page_name": "MrLaptop.vn",
                            "page_profile_picture_url": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.35426-6/434293266_1962626297472535_2644820402052483544_n.jpg?stp=dst-jpg_s60x60&_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHxG4mhMT-mb1FSmpg_kqyRn2GNbWOGzQ-fYY1tY4bND2VOc5LyLXy95XBMfEB59Enznx7Us0cDrNdAtM2itwCW&_nc_ohc=87HeqG5nUjcAb5_HA-N&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfBWcgObYrG3rcbABmFmjU1khX38J6nDCVNBAwdlsP91Jg&oe=6622CFD2",
                            "page_categories": {
                                "199512783398620": "Electronics"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "MrLaptop.vn",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/433060037_1260682638225808_3787351682230697281_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHGs0hpnIbuZ7U9KWUOKhRjbzNnYR_G6AFvM2dhH8boAUQ5mRzfo9EHoy1tpKqox0DUop1a-JeJdGMB65Hk3Uzy&_nc_ohc=lu6Zicydo6sAb42Ih8j&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfCdUurPNSYcsKZm5mwpkzaNIC6LDq1VQMcVHQedEcfl2Q&oe=6622B7CD",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "#Sửa_Laptop, Nâng Cấp 𝐋𝐀𝐏𝐓𝐎𝐏 - 𝐌𝐀𝐂𝐁𝐎𝐎𝐊<br /> 👉Khai Trương Chi Nhánh Mới 𝖦𝗂ảm 30-50%<br /> <br /> 💻Ѕửа mất nɡuồn сһἰ từ 300.000đ<br /> 💻Ѕửа màn һὶnһ сһἰ từ 250.000đ<br /> 💻Nânɡ сấр rаm сһἰ từ 150.000đ<br /> 💻Тһау bàn рһίm сһἰ từ 290.0000đ<br /> 💻Тһау р𝗂n ⅼарtор сһἰ từ 390.000đ<br /> <br /> Bảnɡ ɡ𝗂á: <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fmrlaptop.vn%2Fbang-gia-dich-vu-sua-laptop-lay-lien%2F%3Ffbclid%3DIwAR2aYKErvSwtyWHb-ESVegeqAGOhASZWHFXF9J2_Wc22CX_lAnFVRExo6Qk&amp;h=AT2DKXjx-tR5alINfZGX1WbbDhTk8ztIvQ8FMowwvZANgYcMuemyS1HUlpIN00b3WN3ZRkiEPtxwebzBVfeLW8NcSLBj73Y7mAbRmQwKmQiVREKRqC1xg7IWdLaokkh3b60OcpxtGg\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://mrlaptop.vn/bang-gia-dich-vu-sua-laptop-lay-lien/</a><br /> <br /> 𝐇𝐄̣̂ 𝐓𝐇𝐎̂́𝐍𝐆 𝐒𝐔̛̉𝐀 𝐂𝐇𝐔̛̃𝐀 𝐋𝐀𝐏𝐓𝐎𝐏 - 𝐌𝐀𝐂𝐁𝐎𝐎𝐊 𝐔𝐘 𝐓𝐈́𝐍:<br /> <br /> ✔ СN1: 127 đườnɡ 3/2, Рһườnɡ 11, Ԛuận 10<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: 9һ00-17һ00 - 𝖧оtⅼ𝗂nе: 0931.640.640<br /> <br /> ✔ СN2: 514 Сáсһ Mạnɡ Тһánɡ 8, Р11, Ԛuận 3<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0968.450.450<br /> <br /> ✔ СN3: 167А Đàо 𝖣uу Аnһ, Р9, Рһú Nһuận<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0931.590.590<br /> <br /> ✔ СN4: 203А Ⅼê Ԛuаnɡ Địnһ, Р7, Bὶnһ Тһạnһ<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0934.032.032<br /> <br /> ✔ СN5: 1068B Âu Сơ, Р14, Тân Bὶnһ<br /> (Сửа һànɡ màu đỏ 1068 сó 3 сăn ⅼ𝗂ền kề)<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0936.590.590<br /> <br /> ✔ СN6: 457 Ⅼê 𝖵ăn Тһọ, Р9, 𝖦ò 𝖵ấр<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0966.430.430<br /> <br /> ✔ СN7: 678 Kһа 𝖵ạn Сân, Р. Ⅼ𝗂nһ Đônɡ, Тһủ Đứс<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0962.710.710<br /> <br /> ✔ СN8: 46 𝖣ươnɡ Đὶnһ 𝖧ộ𝗂, Рһướс Ⅼоnɡ B, Тһủ Đứс (Ԛuận 9 сũ)<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0964.260.260<br /> <br /> ✔ СN9: 1020 𝖧ậu 𝖦𝗂аnɡ, Р12, Ԛuận 6<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0923.450.450<br /> <br /> #sửa_laptop  #sửa_macbook #mrlaptop"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "MrLaptop.vn",
                            "disclaimer_label": null,
                            "page_like_count": 5818,
                            "page_profile_uri": "https://facebook.com/mrlaptop.vn",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1711954800,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "1396628347647671",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 6,
                        "collationID": 428692646330024,
                        "currency": "",
                        "endDate": 1713078000,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "1743192135981478",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "MrLaptop.vn",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120208294545770443",
                            "cards": [
                                {
                                    "original_image_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/433225840_991695775917990_7027602308887973426_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeF7A3IFZCxP9VczuQEtyshMgge_uwazUJKCB7-7BrNQklCMsmorm-WpslvC2QOOn-BpL59y9ipY2CVESWpsv-W7&_nc_ohc=v9NGVqB8RFcAb6Hnrgs&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfBEzwKE6EyHwMfUyOOIDY3LLcCnYcELjg6zO45qzAVywA&oe=6622CFDA",
                                    "resized_image_url": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.35426-6/433237813_960236099085316_6668731690366593612_n.jpg?stp=dst-jpg_s600x600&_nc_cat=107&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFYvACOfzwH2fHFGllko4OehqgO0YXIZ5CGqA7RhchnkEtr6gewUT5S0EsIVsbi1338bfCQzCRwZS1HzE0W8ohW&_nc_ohc=PkfRVAOapmMAb77JXJh&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfDlz-eh9mCkDZtVmtP7OlD6dQ6HPwM4ISwg1kfhUKa7hg&oe=6622AD9F",
                                    "watermarked_resized_image_url": "",
                                    "image_crops": {},
                                    "body": " ",
                                    "caption": "fb.com",
                                    "cta_type": "MESSAGE_PAGE",
                                    "cta_text": "Send Message",
                                    "title": "💥NÂNG CẤP RAM LAPTOP",
                                    "link_description": " ",
                                    "link_url": null
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/433099600_1085424872678794_8300321048733327194_n.jpg?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEjSrAjcyhoAciot7lr3ntIsCbLPXJdtvGwJss9cl228Tgbkq98QPfJOKWvkUp2Eme8vnecGl1EhenWEn4HEu5m&_nc_ohc=tAcrxtLKig0Ab5_KiyM&_nc_oc=Adhzb7UU-nswXaoYjb3LmPkXUWWeJwuE_osXYphKF10IRyiSbrgYmKycJ-tCbjaFUmQ&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfDcUEeKANJ4ypNsI2zueUoXsgZDhqiJHgQ64Tc_RetMBw&oe=6622DC88",
                                    "resized_image_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/433192548_397886339621410_2097864651208227824_n.jpg?stp=dst-jpg_s600x600&_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEKqHKwSbvow5MbpgCBcqzhAHgzvGw5fIIAeDO8bDl8gpJAcAvtxYf5fsH-8KdylGCuUjjNgx4KmdACXMBJ25fh&_nc_ohc=5vVcoxSgzDkAb4lDfYt&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfAPtivtuUjZdvdNT9KKL56gv1LyhrpcTKGpg-l1xYt5fA&oe=6622D364",
                                    "watermarked_resized_image_url": "",
                                    "image_crops": {},
                                    "body": " ",
                                    "caption": "fb.com",
                                    "cta_type": "MESSAGE_PAGE",
                                    "cta_text": "Send Message",
                                    "title": "💥THAY BÀN PHÍM LAPTOP",
                                    "link_description": " ",
                                    "link_url": null
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/434570208_1113962869845771_3311379148831770685_n.jpg?_nc_cat=100&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGnZ_LlHoJoviWSKCzpfkQJlOAbsrHTcy2U4BuysdNzLZcybPJ5zxe82FHF67ctS5SAQc1l8GgGBmF6IEMGMN8N&_nc_ohc=rvUhKg_UIKIAb5EABnl&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfBzCwX11eVA-pL_LcW9WryUe5H2mN4_YpJqUHmAlRw-Yg&oe=6622B336",
                                    "resized_image_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/433042467_2364191220442330_3261013073669135371_n.jpg?stp=dst-jpg_s600x600&_nc_cat=110&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEHZ1E42KF0fxpIHMH-51JsqM6s2BvubJCozqzYG-5skJ4zkdTyq5eLSzZTSyWS6-lBE9Fkev_wsZ9CbL9pajXY&_nc_ohc=SrD_2otJF8kAb4ir61Q&_nc_oc=AdgsgqhrSqCuvCvBKjq6RzL37P-a1VA7FwDfmpdsjJjo0L0vaKZRjVcaFwWWOmx5_gg&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfCoOCmmlg3QQdUEiNk_oOHMxg62VIGzcKsHlnd_ubb_uQ&oe=6622D869",
                                    "watermarked_resized_image_url": "",
                                    "image_crops": {},
                                    "body": " ",
                                    "caption": "fb.com",
                                    "cta_type": "MESSAGE_PAGE",
                                    "cta_text": "Send Message",
                                    "title": "💥 THAY PIN LAPTOP",
                                    "link_description": " ",
                                    "link_url": null
                                },
                                {
                                    "original_image_url": "https://scontent.fsgn2-5.fna.fbcdn.net/v/t39.35426-6/433100449_293167213813004_715786345379954496_n.jpg?_nc_cat=104&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFMeXtDmrtCrUUk8JtZ760rRZ0WohIvRItFnRaiEi9Ei_pjWULpYbJbK4h78zFnUYhMbmnZ8VmONXGOUoLhXByj&_nc_ohc=ITE_mSx60vgAb4nZA79&_nc_ht=scontent.fsgn2-5.fna&oh=00_AfCqLRVBlTp1-kv2wQf0zwRDTSZ-dhDOzsRW8puIslnllw&oe=6622CA13",
                                    "resized_image_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/433142297_1473995026659216_5939381791249742040_n.jpg?stp=dst-jpg_s600x600&_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGBdrlwUhI8v1lLpojsKp0XD8g7pDB0O2gPyDukMHQ7aPmkZUYF4Lt3lxwOEKiB29_aOP3d5ZxSwwbVZOVwN0nk&_nc_ohc=w2vn-_SbwoEAb5XfEzM&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfAuhMmG9vznfpYh0WChG4GurgzS_pvsfd3yyPV2QQBo0g&oe=6622C1E8",
                                    "watermarked_resized_image_url": "",
                                    "image_crops": {},
                                    "body": " ",
                                    "caption": "fb.com",
                                    "cta_type": "MESSAGE_PAGE",
                                    "cta_text": "Send Message",
                                    "title": "💥 THAY MÀN HÌNH LAPTOP",
                                    "link_description": " ",
                                    "link_url": null
                                }
                            ],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "carousel",
                            "title": "MrLaptop.vn",
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Địa chỉ của bạn ở đâu?\",\"response\":\"\"},{\"title\":\"Tư vấn sửa laptop\"},{\"title\":\"Báo giá sửa laptop\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"user_edit\":true,\"surface\":\"visual_editor_new\",\"ice_breakers_edited\":true,\"template_id\":\"351556517311891\"}",
                            "images": [],
                            "videos": [],
                            "creation_time": 1711555082,
                            "page_id": 1743192135981478,
                            "page_name": "MrLaptop.vn",
                            "page_profile_picture_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/433186028_805865167786102_5633347964395048166_n.jpg?stp=dst-jpg_s60x60&_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGBUt6BVMOsQjoFO4MLRxcI87hcTx_oATTzuFxPH-gBNGht6F1cH7xEFaCy0hyf3uRg1xDjrOEt3TwZPwOigtsN&_nc_ohc=Y3lAW6_jQssAb6Dc6du&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfArFs_o4JtXNwS72GxuMcsxg0bUsGbyLsiCIDDc9apgkg&oe=6622C811",
                            "page_categories": {
                                "199512783398620": "Electronics"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "MrLaptop.vn",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/433194822_922952809284232_3507543969777883964_n.jpg?_nc_cat=100&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGYkKPWH3C286uhSB92_q6WcAIjf8zesPJwAiN_zN6w8gK-awJyomByVkTdbz-SfB4gDEDNaTq4saE5XaflbnA9&_nc_ohc=zqeJWaH3M-MAb4IuP9b&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfDJhZv5H8G-fdYdJsrUSdTJFJnlT8Wp57ttaSgrQQtMLw&oe=6622D30B",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "#Sửa_Laptop, Nâng Cấp 𝐋𝐀𝐏𝐓𝐎𝐏 - 𝐌𝐀𝐂𝐁𝐎𝐎𝐊<br /> 👉Khai Trương Chi Nhánh Mới 𝖦𝗂ảm 30-50%<br /> <br /> 💻Ѕửа mất nɡuồn сһἰ từ 300.000đ<br /> 💻Ѕửа màn һὶnһ сһἰ từ 250.000đ<br /> 💻Nânɡ сấр rаm сһἰ từ 150.000đ<br /> 💻Тһау bàn рһίm сһἰ từ 290.0000đ<br /> 💻Тһау р𝗂n ⅼарtор сһἰ từ 390.000đ<br /> <br /> Bảnɡ ɡ𝗂á: <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fmrlaptop.vn%2Fbang-gia-dich-vu-sua-laptop-lay-lien%2F%3Ffbclid%3DIwAR2WQXNb2jCtZS38DgxwVeQ-6hEc_Ki7thfpfnuQFLnn7tr9IvoKBDOxRUI&amp;h=AT08I3UVNlMtCP5N8nWhlWBl2Eae9Gz8QkVi0_1fndzytfK53V66iegD36tUkranYkaz_dNZaBzS4UzW6eLq8KMgd7O8buLW7UP_j84udAsvORyC6nMkFpcBMDCgzLturFOVMbEpkQ\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://mrlaptop.vn/bang-gia-dich-vu-sua-laptop-lay-lien/</a><br /> <br /> 𝐇𝐄̣̂ 𝐓𝐇𝐎̂́𝐍𝐆 𝐒𝐔̛̉𝐀 𝐂𝐇𝐔̛̃𝐀 𝐋𝐀𝐏𝐓𝐎𝐏 - 𝐌𝐀𝐂𝐁𝐎𝐎𝐊 𝐔𝐘 𝐓𝐈́𝐍:<br /> <br /> ✔ СN1: 127 đườnɡ 3/2, Рһườnɡ 11, Ԛuận 10<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: 9һ00-17һ00 - 𝖧оtⅼ𝗂nе: 0931.640.640<br /> <br /> ✔ СN2: 514 Сáсһ Mạnɡ Тһánɡ 8, Р11, Ԛuận 3<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0968.450.450<br /> <br /> ✔ СN3: 167А Đàо 𝖣uу Аnһ, Р9, Рһú Nһuận<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0931.590.590<br /> <br /> ✔ СN4: 203А Ⅼê Ԛuаnɡ Địnһ, Р7, Bὶnһ Тһạnһ<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0934.032.032<br /> <br /> ✔ СN5: 1068B Âu Сơ, Р14, Тân Bὶnһ<br /> (Сửа һànɡ màu đỏ 1068 сó 3 сăn ⅼ𝗂ền kề)<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0936.590.590<br /> <br /> ✔ СN6: 457 Ⅼê 𝖵ăn Тһọ, Р9, 𝖦ò 𝖵ấр<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0966.430.430<br /> <br /> ✔ СN7: 678 Kһа 𝖵ạn Сân, Р. Ⅼ𝗂nһ Đônɡ, Тһủ Đứс<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0962.710.710<br /> <br /> ✔ СN8: 46 𝖣ươnɡ Đὶnһ 𝖧ộ𝗂, Рһướс Ⅼоnɡ B, Тһủ Đứс (Ԛuận 9 сũ)<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0964.260.260<br /> <br /> ✔ СN9: 1020 𝖧ậu 𝖦𝗂аnɡ, Р12, Ԛuận 6<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0923.450.450<br /> <br /> #sửa_laptop  #sửa_macbook #mrlaptop"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "MrLaptop.vn",
                            "disclaimer_label": null,
                            "page_like_count": 5818,
                            "page_profile_uri": "https://facebook.com/mrlaptop.vn",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1711954800,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "787772362876727",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 6,
                        "collationID": 952690726573764,
                        "currency": "",
                        "endDate": 1713078000,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "1743192135981478",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "MrLaptop.vn",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120208484968120443",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "image",
                            "title": "💥SỬA LAPTOP GIẢM ĐẾN 50%",
                            "link_description": "Hơn +950.000 Khách hàng đã nhắn tin",
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Địa chỉ của bạn ở đâu?\",\"response\":\"\"},{\"title\":\"Tư vấn sửa laptop\"},{\"title\":\"Báo giá sửa laptop\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"user_edit\":true,\"surface\":\"visual_editor_new\",\"ice_breakers_edited\":true,\"template_id\":\"351556517311891\"}",
                            "images": [
                                {
                                    "original_image_url": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.35426-6/434741641_1959338891201142_7495727187652105738_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeEfBenUAwOlAdZh8mt1hiD_N7gNWzpPyVk3uA1bOk_JWQEavxpj4xMoWV-yBc3AP7eXlsiDAnPVtzs14zzedkRI&_nc_ohc=GgwNHnw2t1sAb7vDj9k&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfA0MaHlD7z7jeJ2V6TtdzgmVO3c0gAuK_MepJr9VVfZgg&oe=6622AC9D",
                                    "resized_image_url": "https://scontent.fsgn2-5.fna.fbcdn.net/v/t39.35426-6/434743570_1333792883926905_2085989893279770568_n.jpg?stp=dst-jpg_s600x600&_nc_cat=104&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGHGnhfXzPGRGvaZovUIw8-xTmZKutBPOLFOZkq60E84gnEvDzRrga4phLFbRBkIiCXxhJthORgXV38N4pQdvVy&_nc_ohc=djoy0gmrNysAb6kwzSZ&_nc_ht=scontent.fsgn2-5.fna&oh=00_AfAFeqkGhpZAcVnNY6_9I6aJvGcdc-AOXyBwPFjK0Cp3gg&oe=6622BB4C",
                                    "watermarked_resized_image_url": "",
                                    "image_crops": {}
                                }
                            ],
                            "videos": [],
                            "creation_time": 1711983224,
                            "page_id": 1743192135981478,
                            "page_name": "MrLaptop.vn",
                            "page_profile_picture_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/434746790_1098938394747786_1149265548702220559_n.jpg?stp=dst-jpg_s60x60&_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeE9nOqWNJUNDNhSkGLejKE_xDdKAlyjS3XEN0oCXKNLdYaWERAG6UkxsP7eAuRfASoiE2Mhp0N1bAQ8OpFdKHPe&_nc_ohc=zzfXMGWEjJkAb6xcU77&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfD9Gse8o4pDxk-ObmGQo7lKEiOcZYIl673d0yMvawHWPA&oe=6622B9B6",
                            "page_categories": {
                                "199512783398620": "Electronics"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "MrLaptop.vn",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/434745948_1585192038979972_4418164544298173204_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeExJ4yXHGlML7LR2JSI5EQXuklqNsK0D_u6SWo2wrQP-wkfIaqZcMpEURoWF2lWkIyQ2kkbXMd7AGwAkwUqnYfm&_nc_ohc=Cmoov_IkCsMAb5ok9lx&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfDsy8RtT9SoU-HXop4fKBNc4vCyjifPpiNWyNkdeokCPg&oe=6622B863",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "#Sửa_Laptop, Nâng Cấp 𝐋𝐀𝐏𝐓𝐎𝐏 - 𝐌𝐀𝐂𝐁𝐎𝐎𝐊<br /> 👉Khai Trương Chi Nhánh Mới 𝖦𝗂ảm 30-50%<br /> <br /> 💻Ѕửа mất nɡuồn сһἰ từ 300.000đ<br /> 💻Ѕửа màn һὶnһ сһἰ từ 250.000đ<br /> 💻Nânɡ сấр rаm сһἰ từ 150.000đ<br /> 💻Тһау bàn рһίm сһἰ từ 290.0000đ<br /> 💻Тһау р𝗂n ⅼарtор сһἰ từ 390.000đ<br /> <br /> Bảnɡ ɡ𝗂á: <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fmrlaptop.vn%2Fbang-gia-dich-vu-sua-laptop-lay-lien%2F%3Ffbclid%3DIwAR2wFgSPJniDMbFZZhEm3y3czSKX7JTq4lnTfcEn4se6pJFm6fTZ4O6UEMM&amp;h=AT0dxEYetGSQKnJXe-XOS9PLAfDAbb7hNJa8mEKtFfmWHJIY54YvgxrpLESqeMsAIgeEJccvaUEYKhKDcskx628eCyrNOHnLtQXEuAodWN2KCAKDZ7dm2aq4Zzk9kKc0U6ivCw9ljA\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://mrlaptop.vn/bang-gia-dich-vu-sua-laptop-lay-lien/</a><br /> <br /> 𝐇𝐄̣̂ 𝐓𝐇𝐎̂́𝐍𝐆 𝐒𝐔̛̉𝐀 𝐂𝐇𝐔̛̃𝐀 𝐋𝐀𝐏𝐓𝐎𝐏 - 𝐌𝐀𝐂𝐁𝐎𝐎𝐊 𝐔𝐘 𝐓𝐈́𝐍:<br /> <br /> ✔ СN1: 127 đườnɡ 3/2, Рһườnɡ 11, Ԛuận 10<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: 9һ00-17һ00 - 𝖧оtⅼ𝗂nе: 0931.640.640<br /> <br /> ✔ СN2: 514 Сáсһ Mạnɡ Тһánɡ 8, Р11, Ԛuận 3<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0968.450.450<br /> <br /> ✔ СN3: 167А Đàо 𝖣uу Аnһ, Р9, Рһú Nһuận<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0931.590.590<br /> <br /> ✔ СN4: 203А Ⅼê Ԛuаnɡ Địnһ, Р7, Bὶnһ Тһạnһ<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0934.032.032<br /> <br /> ✔ СN5: 1068B Âu Сơ, Р14, Тân Bὶnһ<br /> (Сửа һànɡ màu đỏ 1068 сó 3 сăn ⅼ𝗂ền kề)<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0936.590.590<br /> <br /> ✔ СN6: 457 Ⅼê 𝖵ăn Тһọ, Р9, 𝖦ò 𝖵ấр<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0966.430.430<br /> <br /> ✔ СN7: 678 Kһа 𝖵ạn Сân, Р. Ⅼ𝗂nһ Đônɡ, Тһủ Đứс<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0962.710.710<br /> <br /> ✔ СN8: 46 𝖣ươnɡ Đὶnһ 𝖧ộ𝗂, Рһướс Ⅼоnɡ B, Тһủ Đứс (Ԛuận 9 сũ)<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0964.260.260<br /> <br /> ✔ СN9: 1020 𝖧ậu 𝖦𝗂аnɡ, Р12, Ԛuận 6<br /> - Тһứ 2-7: 8һ30-18һ30 - СN: Nɡһἰ- 𝖧оtⅼ𝗂nе: 0923.450.450<br /> <br /> #sửa_laptop  #sửa_macbook #mrlaptop"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "MrLaptop.vn",
                            "disclaimer_label": null,
                            "page_like_count": 5818,
                            "page_profile_uri": "https://facebook.com/mrlaptop.vn",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1711954800,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "771529591753503",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 1,
                        "collationID": 427561616401119,
                        "currency": "",
                        "endDate": 1713078000,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "107189848084236",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "Trung Tâm Laptop Hải Phòng",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120207228610870345",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": "LAPTOP DELL INSPIRON 3511",
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": null,
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t42.1790-2/10000000_771529611753501_6924560009579507299_n.?_nc_cat=101&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeERxZ-JbY8n8rsHuC_ma9NQ-W27eqGa5735bbt6oZrnvZNhr2fQXyQOFEi2dPhvHNpshJJJcsNNkh2VghTncMvd&_nc_ohc=rxAaBztzojIAb5Qpb5a&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfBeIwNjTJRtBM-cVV76kiOdZYOr6MM9vvLRo2y_icevZw&oe=6622A593",
                                    "video_sd_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t42.1790-2/433133607_930016725257213_3761929206263562987_n.mp4?_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGhOtcrOGDgI-C7qaAW4a-BFIcYu0qOVNQUhxi7So5U1L664eUb6fIgStH1oyFSHmKYM8aj4XbzeNstyW9_c66Z&_nc_ohc=sfhwgjwRnQ0Ab7E4ijp&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfAY8S09dN8zr2oe-A2kTuCnOBstMaxUo8oGDoXVkOh79Q&oe=6622C951",
                                    "watermarked_video_sd_url": "",
                                    "watermarked_video_hd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/433185882_429779162829712_3081569331243015784_n.jpg?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGRQzhrhGi9FqLOFVggJqudEFPbs2F_26oQU9uzYX_bqqiDr-qZRnFOcTiyv57sDZgmOz2fgdyWcwXx3F5zgQ03&_nc_ohc=luI5K4QMn10Ab6L7Z05&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfCWhNsDJCo5HJTjrwwPcsoZs-0HTjqW3s5c5y2vV8BdrA&oe=6622C9CE"
                                }
                            ],
                            "creation_time": 1710557718,
                            "page_id": 107189848084236,
                            "page_name": "Trung Tâm Laptop Hải Phòng",
                            "page_profile_picture_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.35426-6/432583544_960347899041140_6621744717932202823_n.jpg?stp=dst-jpg_s60x60&_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFFmauFiZBz8L7DsXzEP45zuI-KiwINxIu4j4qLAg3Ei2Cnrz2nKcdntIDgFQY0bUI71ejoKPnFR5oWdVI8sWt_&_nc_ohc=pkfllIpP9kQAb5XGHNG&_nc_oc=AdhyWXlYoAnL-F79cXOdTMgbLrN4B8bZRyt7cLN6XHNZoAGNsUapRcrhhAKRObTax4s&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfB9mrt55rPdnn49FFg98hJDlG4Swtp0eGNFNA7K9u1BWQ&oe=6622A7C9",
                            "page_categories": {
                                "200600219953504": "Shopping"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "Trung Tâm Laptop Hải Phòng",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/433070012_1421968021756353_6896405659334153691_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHsLqfiIXp14IxghOuim5GSKs62vN8fNsQqzra83x82xLAm81mnsiSMhMTe3QekvVT_2W9ueLnksQ7hiaLpHAdS&_nc_ohc=CujTU_dCsb8Ab7r1tk1&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfC74iq6zEqZJ0qLXAJbSUs2pxD12NCwRymcHzRO_6efgA&oe=6622D104",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "🔥𝐋𝐀𝐏𝐓𝐎𝐏 𝐃𝐄𝐋𝐋 𝐈𝐍𝐒𝐏𝐈𝐑𝐎𝐍 𝟑𝟓𝟏𝟏 ( 𝐍𝐄𝐖 𝟏𝟎𝟎% ) | Cứng cáp , chắc chắn ,CPU thế hệ 11 &gt;&gt;&gt; 😱😱<br /> ⚠️ 𝑺𝒂𝒍𝒆 𝒔𝒂̣̂𝒑 𝒔𝒂̀𝒏 𝒈𝒊𝒂̉𝒎 𝒏𝒈𝒂𝒚 𝒄𝒉𝒊̉ 𝒄𝒐̀𝒏 #11trxxx<br /> ------------------------------------<br /> 🔰𝐿𝑎𝑝𝑡𝑜𝑝 𝐷𝑒𝑙𝑙 𝐼𝑛𝑠𝑝𝑖𝑟𝑜𝑛 3511 | 𝐼5 - 1135𝐺7 | 𝑟𝑎𝑚 16𝐺𝐵 | 𝑠𝑠𝑑 512𝐺𝐵 | 15.6 &#039;&#039; 𝐹𝐻𝐷 <br /> <br /> 📌 Ngoại hình đẹp , hiệu năng khoẻ , phục vụ thoải mái nhu cầu học tập , làm việc , đồ hoạ 2D hay giải trí hàng ngày cho AE đều ok luôn nhé <br /> <br /> ↪️ Ae inbox để được tư vấn ngay nhé !!!<br /> -------------------------------<br /> 𝑯𝒂̉𝒊 𝑷𝒉𝒐̀𝒏𝒈 𝑪𝒐𝒎𝒑𝒖𝒕𝒆𝒓 - 𝑻𝒉𝒆̂́ 𝒈𝒊𝒐̛́𝒊 𝒄𝒐̂𝒏𝒈 𝒏𝒈𝒉𝒆̣̂ 𝒕𝒂̣𝒊 𝑯𝒂̉𝒊 𝑷𝒉𝒐̀𝒏𝒈<br /> 🎁 Tặng ngay Combo Quà tặng or Voucher #200k<br /> ✨ Hỗ trợ trả góp ngay +Đổi mới 15 ngày đầu+Free phần mềm ,vệ sinh<br /> 🏡Địa chỉ : 82-84 Quán Nam, Kênh Dương, Lê Chân, Hải Phòng<br />  ☎ Hotline : 0981.919.595<br /> 🌍 Website : <a href=\"https://l.facebook.com/l.php?u=http%3A%2F%2Fmaytinhhaiphong.com%2F%3Ffbclid%3DIwAR3Ojdq4BDM8-UQ_YFsXyeOua01KdOCNfXb7tf6lu6_KOw1eFNOESXec62k&amp;h=AT0oN_e0xVtdzNL8YS0rQj2eejsI6KOp0xmbGmVvG1l7gtZ3KiFEJe97yPhbWrOifrCI3lAENJ71nSPJItffi4PUE_iSbfaI-XqNaDCkekQ2jHvqlj-xRLHxFMqMsrbCziKGHOtw6w\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">maytinhhaiphong.com</a>"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "Trung Tâm Laptop Hải Phòng",
                            "disclaimer_label": null,
                            "page_like_count": 5502,
                            "page_profile_uri": "https://facebook.com/100091314824136",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1710486000,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ],
                [
                    {
                        "adid": "0",
                        "adArchiveID": "386333370850856",
                        "archiveTypes": [],
                        "categories": [
                            0
                        ],
                        "containsDigitallyCreatedMedia": false,
                        "containsSensitiveContent": false,
                        "collationCount": 3,
                        "collationID": 1357882628477480,
                        "currency": "",
                        "endDate": 1713078000,
                        "entityType": "person_profile",
                        "fevInfo": null,
                        "gatedType": "eligible",
                        "hasUserReported": false,
                        "hiddenSafetyData": false,
                        "hideDataStatus": "NONE",
                        "impressionsWithIndex": {
                            "impressionsText": null,
                            "impressionsIndex": -1
                        },
                        "isAAAEligible": false,
                        "isActive": true,
                        "isProfilePage": false,
                        "pageID": "1743192135981478",
                        "pageInfo": null,
                        "pageIsDeleted": false,
                        "pageName": "MrLaptop.vn",
                        "politicalCountries": [],
                        "reachEstimate": null,
                        "reportCount": null,
                        "snapshot": {
                            "ad_creative_id": "120208295621010443",
                            "cards": [],
                            "body_translations": {},
                            "byline": null,
                            "caption": null,
                            "cta_text": "Gửi tin nhắn",
                            "dynamic_item_flags": {},
                            "dynamic_versions": null,
                            "edited_snapshots": [],
                            "effective_authorization_category": "NONE",
                            "event": [],
                            "extra_images": [],
                            "extra_links": [],
                            "extra_texts": [],
                            "extra_videos": [],
                            "instagram_shopping_products": [],
                            "display_format": "video",
                            "title": "Hơn +950.000 KH đã nhắn tin sửa laptop",
                            "link_description": null,
                            "link_url": null,
                            "page_welcome_message": "{\"type\":\"VISUAL_EDITOR\",\"version\":2,\"landing_screen_type\":\"welcome_message\",\"media_type\":\"text\",\"text_format\":{\"customer_action_type\":\"ice_breakers\",\"message\":{\"ice_breakers\":[{\"title\":\"Địa chỉ của bạn ở đâu?\",\"response\":\"\"},{\"title\":\"Tư vấn sửa laptop\"},{\"title\":\"Báo giá sửa laptop\"}],\"quick_replies\":[],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"image_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"template\",\"payload\":{\"template_type\":\"generic\",\"elements\":[{\"title\":\"\",\"buttons\":[]}]}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"video_format\":{\"customer_action_type\":\"quick_replies\",\"message\":{\"attachment\":{\"type\":\"video\",\"payload\":{\"attachment_id\":\"\"}},\"quick_replies\":[{\"title\":\"Tôi muốn tìm hiểu thêm\",\"content_type\":\"text\"}],\"text\":\"Chào {{user_first_name}}! Chúng tôi có thể giúp gì cho bạn?\"}},\"user_edit\":true,\"surface\":\"visual_editor_new\",\"ice_breakers_edited\":true,\"template_id\":\"351556517311891\"}",
                            "images": [],
                            "videos": [
                                {
                                    "video_hd_url": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t42.1790-2/434613709_957205155975840_315204893304043429_n.?_nc_cat=102&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGI3_-F5OZgYOsTurUksVSBfIJ9tIcGGQ18gn20hwYZDYLIYYuyVsxdo-laJMpIsr5NKNYcHEKB5kyYvq2GCvud&_nc_ohc=FH7zmQXeTAcAb4rXqPQ&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfCFlE5vL8DjCHVREjwlRWbPPpDH6HoqrpIcI_kMkip8Lg&oe=6622C7E1",
                                    "video_sd_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t42.1790-2/377486452_1028565955012792_2780075476561710982_n.mp4?_nc_cat=100&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeGjnChlR7vRDfpxm926-ccu3DFkSXieD_DcMWRJeJ4P8EvEoieZYMKVMTyLCwSvdlcVvgWNMLHkBzeYzVHGcd9c&_nc_ohc=cYb7qHEw7VwAb4NCjs1&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfBxdnvDyR6-Ng9VRsN4bj0L__Nf6PHafLy7y0VbcygAcQ&oe=6622C995",
                                    "watermarked_video_sd_url": "",
                                    "watermarked_video_hd_url": "",
                                    "video_preview_image_url": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.35426-6/433938176_800797508739460_193479137148593180_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeFzQmlQMtTJDbkZm37nEKACN37OKY1fCYo3fs4pjV8JisDNU-WAbMMT6YDLSxmT6PpWZSYcnxbJ8ZgHLA-iJk47&_nc_ohc=c9qrqEdbGcMAb6uw8xM&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfB98FTwoIDj-_cvdUOSwXJCT-lXxyqCP1hnAgSJPVNg3A&oe=6622C7B9"
                                }
                            ],
                            "creation_time": 1711556723,
                            "page_id": 1743192135981478,
                            "page_name": "MrLaptop.vn",
                            "page_profile_picture_url": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.35426-6/434024077_1132516901223813_190830448826146690_n.jpg?stp=dst-jpg_s60x60&_nc_cat=108&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeF02KSKAPiWeTnkgXfE5KrVTfnkWEkAbIRN-eRYSQBshJL-k5lxcd2VBTkhZkJRDAwfQxUMTRelF244hkMcfh-0&_nc_ohc=IPFLdA6MHU0Ab4hR9My&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfBO2jpY8byZztHEpOSmk-H3Kf65NHirSnXrTbE4RvTXDg&oe=6622A7EF",
                            "page_categories": {
                                "199512783398620": "Electronics"
                            },
                            "page_entity_type": "person_profile",
                            "page_is_profile_page": false,
                            "instagram_actor_name": "MrLaptop.vn",
                            "instagram_profile_pic_url": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.35426-6/433886168_950139923566287_228801619673642815_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=c53f8f&_nc_eui2=AeHMxlbj0LgyW4F_txKldCCSpAk6Za9Sm56kCTplr1Kbno1xONqKwoJPnqhR8mlryHdtik_TEvk6-Dd5Afve6LrX&_nc_ohc=Oo66uLXoXAMAb41uMMV&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfDOCFJLGTixob_pEWtrG4Niok0sEcCBhtNBtz_PtzfQtw&oe=6622BFA6",
                            "instagram_url": "",
                            "instagram_handle": "",
                            "is_reshared": false,
                            "version": 3,
                            "body": {
                                "context": {},
                                "markup": {
                                    "__html": "Sửa Chữa, Nâng Cấp #LAPTOP - #MACBOOK - Lấy Liền Giá Rẻ, Xem Trực Tiếp<br /> 👉𝖦𝗂ảm  30-50% сһо ѕ𝗂nһ v𝗂ên tạ𝗂 ТР.𝖧СM<br /> <br /> 💻Ѕửа mất nɡuồn сһἰ từ 300.000đ<br /> 💻Ѕửа màn һὶnһ сһἰ từ 250.000đ<br /> 💻Nânɡ сấр rаm сһἰ từ 150.000đ<br /> 💻Тһау bàn рһίm сһἰ từ 290.0000đ<br /> 💻Тһау р𝗂n ⅼарtор сһἰ từ 390.000đ<br /> <br /> Хеm tһêm bảnɡ ɡ𝗂á: <a href=\"https://l.facebook.com/l.php?u=https%3A%2F%2Fmrlaptop.vn%2Fbang-gia-dich-vu-sua-laptop-lay-lien%2F%3Ffbclid%3DIwAR1r7_XsZTc_KsvTRrBYSA7mG_LAbd2_eg915rC5zmpyJNF7KgF-Wm1Ruv4&amp;h=AT3nAx89E8aYJjGqbKlRhJ_uuCwY_R6CL8kGUJHyM2TS3Jf_KFzJ_lac5Sq4Jawmaus2S3IW0isFsxkmd9vPLH9cmvSEmFVxr9wtnL0Lc47XBbjRz1zBLPwsj6BbbA-sUku_mS_N9A\" rel=\"nofollow noreferrer\" target=\"_blank\" data-lynx-mode=\"asynclazy\">https://mrlaptop.vn/bang-gia-dich-vu-sua-laptop-lay-lien/</a><br /> <br /> Ⅼàm v𝗂ệс: 8һ30 đến 6һ30 (Тһứ 2 -7)<br /> Сһủ nһật: сһἰ ⅼàm сһ𝗂 nһánһ Ԛ10 (9һ đến 17һ00)<br /> 𝖦ọ𝗂  0931.640.640 báо ɡ𝗂á nһаnһ<br /> <br /> 𝖧Ệ Т𝖧ỐN𝖦 ЅỬА С𝖧ỮА ⅬАРТОР - MАСBООK 𝖴𝖸 ТÍN:<br /> ✔ СN1: 127 đườnɡ 3/2, Рһườnɡ 11, Ԛuận 10<br /> ✔ СN2: 514 СMТ8, Р11, Ԛuận 3<br /> ✔ СN3: 167А Đàо 𝖣uу Аnһ, Р9, Рһú Nһuận (Nɡау nɡã 3 Рһổ Ԛuаnɡ - Đàо 𝖣uу Аnһ)<br /> ✔ СN4: 203А Ⅼê Ԛuаnɡ Địnһ, Р14, Bὶnһ Тһạnһ<br /> ✔ СN5: 1068B Âu Сơ, Р14, Тân Bὶnһ (𝖦ần Âu Сơ - Тrườnɡ Сһ𝗂nһ)<br /> ✔ СN6: 457 Ⅼê 𝖵ăn Тһọ, Р9, 𝖦ò 𝖵ấр<br /> ✔ СN7: 678 Kһа 𝖵ạn Сân, Ⅼ𝗂nһ Đônɡ Тһủ Đứс<br /> ✔ СN8: 46 𝖣ươnɡ Đὶnһ 𝖧ộ𝗂, Рһướс Ⅼоnɡ B, Тһủ Đứс (Ԛuận 9 сũ, ɡ𝗂ао vớ𝗂 Đỗ Хuân 𝖧ợр)"
                                },
                                "callerHash": "6506f381dd66c00c3f81a269693ae295"
                            },
                            "brazil_tax_id": null,
                            "branded_content": null,
                            "current_page_name": "MrLaptop.vn",
                            "disclaimer_label": null,
                            "page_like_count": 5818,
                            "page_profile_uri": "https://facebook.com/mrlaptop.vn",
                            "page_is_deleted": false,
                            "root_reshared_post": null,
                            "cta_type": "MESSAGE_PAGE",
                            "additional_info": null,
                            "ec_certificates": null,
                            "country_iso_code": null,
                            "instagram_branded_content": null
                        },
                        "spend": null,
                        "startDate": 1711522800,
                        "stateMediaRunLabel": null,
                        "publisherPlatform": [
                            "facebook",
                            "instagram",
                            "audience_network",
                            "messenger"
                        ],
                        "menuItems": []
                    }
                ]
            ],
            "pageResults": [],
            "forwardCursor": "AQHRqvX6WbZS6b4cbAb4DjCqAH8dlFTUMlH77NzcF05AFtRoOIyLmv4nHbMkeTbCGjMP",
            "backwardCursor": "",
            "totalCount": 50001,
            "collationToken": "a8aaf6eb-0cd9-4789-b45d-60c031263d39"
        },
        "jsmods": {
            "define": [
                [
                    "cr:1078",
                    [],
                    {
                        "__rc": [
                            null,
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:1080",
                    [
                        "unexpectedUseInComet"
                    ],
                    {
                        "__rc": [
                            "unexpectedUseInComet",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:1126",
                    [
                        "TimeSliceImpl"
                    ],
                    {
                        "__rc": [
                            "TimeSliceImpl",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:7736",
                    [
                        "FBLynxLogging"
                    ],
                    {
                        "__rc": [
                            "FBLynxLogging",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:7936",
                    [
                        "BlueCompatRouter"
                    ],
                    {
                        "__rc": [
                            "BlueCompatRouter",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:708886",
                    [
                        "EventProfilerImpl"
                    ],
                    {
                        "__rc": [
                            "EventProfilerImpl",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:310",
                    [
                        "RunWWW"
                    ],
                    {
                        "__rc": [
                            "RunWWW",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:6640",
                    [
                        "PromiseImpl"
                    ],
                    {
                        "__rc": [
                            "PromiseImpl",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:7385",
                    [
                        "clearIntervalWWW"
                    ],
                    {
                        "__rc": [
                            "clearIntervalWWW",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:7386",
                    [
                        "clearTimeoutWWW"
                    ],
                    {
                        "__rc": [
                            "clearTimeoutWWW",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:7389",
                    [
                        "setIntervalAcrossTransitionsWWW"
                    ],
                    {
                        "__rc": [
                            "setIntervalAcrossTransitionsWWW",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:7390",
                    [
                        "setTimeoutWWW"
                    ],
                    {
                        "__rc": [
                            "setTimeoutWWW",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:7391",
                    [
                        "setTimeoutAcrossTransitionsWWW"
                    ],
                    {
                        "__rc": [
                            "setTimeoutAcrossTransitionsWWW",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:7730",
                    [
                        "getFbtResult"
                    ],
                    {
                        "__rc": [
                            "getFbtResult",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:8906",
                    [
                        "goURIWWW"
                    ],
                    {
                        "__rc": [
                            "goURIWWW",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:8958",
                    [
                        "FBJSON"
                    ],
                    {
                        "__rc": [
                            "FBJSON",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:8959",
                    [
                        "DTSG"
                    ],
                    {
                        "__rc": [
                            "DTSG",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:8960",
                    [
                        "DTSG_ASYNC"
                    ],
                    {
                        "__rc": [
                            "DTSG_ASYNC",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:696703",
                    [],
                    {
                        "__rc": [
                            null,
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:6799",
                    [
                        "EventProfilerAdsSessionProvider"
                    ],
                    {
                        "__rc": [
                            "EventProfilerAdsSessionProvider",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:1290",
                    [],
                    {
                        "__rc": [
                            null,
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:8828",
                    [],
                    {
                        "__rc": [
                            null,
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:1094907",
                    [],
                    {
                        "__rc": [
                            null,
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:925100",
                    [
                        "RunBlue"
                    ],
                    {
                        "__rc": [
                            "RunBlue",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:1003267",
                    [
                        "clearIntervalBlue"
                    ],
                    {
                        "__rc": [
                            "clearIntervalBlue",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:806696",
                    [
                        "clearTimeoutBlue"
                    ],
                    {
                        "__rc": [
                            "clearTimeoutBlue",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:896462",
                    [
                        "setIntervalAcrossTransitionsBlue"
                    ],
                    {
                        "__rc": [
                            "setIntervalAcrossTransitionsBlue",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:807042",
                    [
                        "setTimeoutBlue"
                    ],
                    {
                        "__rc": [
                            "setTimeoutBlue",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:986633",
                    [
                        "setTimeoutAcrossTransitionsBlue"
                    ],
                    {
                        "__rc": [
                            "setTimeoutAcrossTransitionsBlue",
                            null
                        ]
                    },
                    -1
                ],
                [
                    "cr:1183579",
                    [
                        "InlineFbtResultImpl"
                    ],
                    {
                        "__rc": [
                            "InlineFbtResultImpl",
                            null
                        ]
                    },
                    -1
                ]
            ],
            "require": [
                [
                    "FBLynx@d864349aa89d1e747ec2339815f64013",
                    "setupDelegation",
                    [],
                    []
                ],
                [
                    "FbtLogging@3f90e710c89d65ee3ffd0177e50fb51d"
                ],
                [
                    "IntlQtEventFalcoEvent@3f90e710c89d65ee3ffd0177e50fb51d"
                ],
                [
                    "RequireDeferredReference@8ca629add99dfccc979fe850af3eed9a",
                    "unblock",
                    [],
                    [
                        [
                            "FbtLogging",
                            "IntlQtEventFalcoEvent"
                        ],
                        "sd"
                    ]
                ],
                [
                    "RequireDeferredReference@8ca629add99dfccc979fe850af3eed9a",
                    "unblock",
                    [],
                    [
                        [
                            "FbtLogging",
                            "IntlQtEventFalcoEvent"
                        ],
                        "css"
                    ]
                ]
            ]
        },
        "hsrp": {
            "hsdp": {
                "clpData": {
                    "1838142": {
                        "r": 1,
                        "s": 1
                    },
                    "1837559": {
                        "r": 1
                    },
                    "1848815": {
                        "r": 10000,
                        "s": 1
                    }
                },
                "gkxData": {
                    "25572": {
                        "result": false,
                        "hash": null
                    },
                    "20935": {
                        "result": false,
                        "hash": null
                    },
                    "7742": {
                        "result": false,
                        "hash": null
                    },
                    "20936": {
                        "result": false,
                        "hash": null
                    },
                    "20939": {
                        "result": true,
                        "hash": null
                    },
                    "21043": {
                        "result": false,
                        "hash": null
                    },
                    "25571": {
                        "result": false,
                        "hash": null
                    },
                    "20836": {
                        "result": false,
                        "hash": null
                    },
                    "20948": {
                        "result": true,
                        "hash": null
                    }
                },
                "justknobxData": {
                    "2269": {
                        "r": false
                    }
                }
            },
            "hblp": {
                "consistency": {
                    "rev": 1012776817
                },
                "rsrcMap": {
                    "4ICgmNm": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yP/r/OUZiA28Uqln.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeG3ufNjeyndSDw3kUIjnSWTD9r4Mo9gRocP2vgyj2BGh_MCgpM_C2RoflgvNYVKQkEqyYPOCQLRo54alMryNxeF"
                    },
                    "e8KbigC": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3iFy44/yq/l/vi_VN/zqHWvGXpabZ.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeFg_OYpX4mczOQWeUPYuKYS7yi3TQJYlEXvKLdNAliURbDHF8hkfeUvE6gks1IBZCmv3k60Xmn_XzCwWeUvjWDs"
                    },
                    "BiRHLnG": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/ya/r/izTZY5sqWJT.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeFH_l8k206kO0swS_JB8O78Z55ORmC_wOVnnk5GYL_A5bfKiVLX6ouw5YIHKhOLHANxvB6zNirfdHZjiNNjOZqo"
                    },
                    "d37yUGn": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yo/r/YvbwYOOvPhl.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeHiK9rn2zvHxtfyEDkeV8OkO0thtVLMthY7S2G1Usy2FqF_uxQhw6w3gMknhbCRQqhXobX5by0R-chMcBW8l_JC"
                    },
                    "9bDSwfT": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3i2x04/yZ/l/vi_VN/cmH3EJYu0aj.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeE0AMpet6__gI8MwfTS7YaR8Ska92RswOLxKRr3ZGzA4j4LANsV_SiuAS3nUg3WbKaDBPQDCTKGsFpJQAzhxOft"
                    },
                    "UmHNvtz": {
                        "type": "css",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yo/l/0,cross/oI7bhS_irZs.css?_nc_x=z9VIGQBJZK9&_nc_eui2=AeEL57363t6A7Z5sMix2nYRi_AlBkAbrnQX8CUGQBuudBTmIWOFStTYnKVvFTk47HWwTj-8C2JZj7xH_Kve27mQC"
                    },
                    "LVchrHd": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yl/r/f7u7E5VeHqa.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeEjgwQcuIM3re5DymCq3EQpUcGr99BXRyNRwav30FdHI3P156vy-2rmmr6NCCIFORmAmNpJe9_eb2PyGsPaD-Dp"
                    },
                    "kvx582Y": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yK/r/jMaPOqcTw38.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeG4767cICBFiFI1SPJ_LAJQmDgt4UTnoyuYOC3hROejKwLZVOFQqFo4xfkK9fLynmMGk11_0pX0vHGNgvQaRrBZ"
                    },
                    "3HNSMZt": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/y4/r/xPI18UMP6Nr.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeGPWG6At2edANcPjktIW2cHM4yisnr7q7YzjKKyevurtkpFp6Ot4RDZH8OxDaEymUvF2LizqZ1fQd_SRZpfZHJG"
                    },
                    "Hdg+cXJ": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yE/r/KqVnbuezAjj.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeG3kX4iZlfFzgGaBDrQg8IMxt1FoHdJlavG3UWgd0mVq08hzU_JICkZtzZWJoMrwwDq3l1_6Jp2kTeENoI157oy"
                    },
                    "0TAmMmp": {
                        "type": "css",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yy/l/0,cross/Qe3QBVgtXHk.css?_nc_x=z9VIGQBJZK9&_nc_eui2=AeGEyE2lCwxaYWgrHIGh4ewj3ARJ8eKUsfzcBEnx4pSx_IoHO7b1JwUXWv9_6ivx74sSas6xZsfOdNDDSoS2n3BW"
                    },
                    "IYvn1RJ": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yq/r/5yJsr6VAAbw.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeEGJ-cfXaobBX4HfsxDB15fSA1wb-Gu3Z5IDXBv4a7dnkg73f1ueXwpgsiP2tx9I5f0wjGtfoahYoAh6CiPn2-C"
                    },
                    "qUOfXdB": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3iJ044/yA/l/vi_VN/RqRdOlyZWMv.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeHkh4mjuwAMJeetEFoPM593EP51FjVYQcUQ_nUWNVhBxbgRhL8hrAcOWtXstbQpbCntxXHMk1BTqow_VKbaw_Hf"
                    },
                    "bB8N6Cz": {
                        "type": "css",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yr/l/0,cross/nuNKxsHxWy3.css?_nc_x=z9VIGQBJZK9&_nc_eui2=AeF58W2w46mff1C_vC434C4nesyItZ2lUuh6zIi1naVS6EJbu3eE1NYFWzhLl6j0gDezZiPKXrp3ctYHgdyT29xr"
                    },
                    "R5w1rCJ": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yF/r/p55HfXW__mM.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeEl4KZ7vgtQ08z5tkreZOpjJd9I1A5T1XIl30jUDlPVckm5XggdhmjliiNf73ji9d4Fsx2EAn-bZS1ZEw38wI9g"
                    },
                    "Ufq6YWX": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yX/r/eGY_1gEOdFg.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeHun5aEDdfMYtBk_T5eiXm7Jup5DAj_2uYm6nkMCP_a5i6UEgvZfushTxz6awqim1CeiKjWteGgGnIENuGhpnc7"
                    },
                    "Wsv7q+J": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yg/r/hwTPgdqWo6P.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeF3eQA3JSjsQcNyG7MmpDpYeLhcFdBQsFV4uFwV0FCwVRDEL0oK14v8DpqFqSOFamIbF3-1gKMTGKWe9sYiFc22"
                    },
                    "LbsdIZo": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yB/r/FZobwhnpqXb.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeFWSqmptR9mKCDQ-SJyXovEVsEPZF0YhvxWwQ9kXRiG_B0A2AH0KPGJ0gST77iUq4lo6P_q3bVjT9EfMinvJgf3"
                    },
                    "7+vJC3A": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3iWPy4/yM/l/vi_VN/gj8rdc27aw8.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeFkUNX-4D5W-rdC09YfASN1GdLAKbe4asIZ0sApt7hqwps85JZ-_0IJxEDI74SHQEMYmVjAhSoPhSGpNDsMTZR-"
                    },
                    "UHub1Gz": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3i-pX4/yX/l/vi_VN/kSepFcXZ4Rc.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeGWqrpgvGeGxseW1YbHHX2HJeT0OURKVYYl5PQ5REpVhjJGQ9vN5_CFRUQc5hGCkIlulfbcA6rdJNZ6FuRdvn97"
                    },
                    "zaGHrql": {
                        "type": "css",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yn/l/0,cross/DrNg0Fyi_Jx.css?_nc_x=z9VIGQBJZK9&_nc_eui2=AeG_aK9_5pV2BjgnMTy3_AU60VF7vbVF4WTRUXu9tUXhZOZ6N2l8BNcy5b5GbVG_3koGKHcqaI4nywAdlvbZpJZx"
                    },
                    "rk/b7Sj": {
                        "type": "css",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yb/l/0,cross/aS5oSok2AlP.css?_nc_x=z9VIGQBJZK9&_nc_eui2=AeGkBYzmr6c6uB0QpICMXWWI6C29sJxbCBfoLb2wnFsIF97amhtV_LXXR2S9c_bQRmzT5Wh5fm3RLA6QCtFz7OdE"
                    },
                    "MJUxMvv": {
                        "type": "css",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yE/l/0,cross/BBm7ueph0Ce.css?_nc_x=z9VIGQBJZK9&_nc_eui2=AeFdIZOP4YuV2vLLF2HenFeJ_CHBXc5CoG38IcFdzkKgbcJm51Gn7LmYxzXk_k5BOcAINynUMZ61uQkqnYJq1ONy"
                    },
                    "2IRmU7r": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3iois4/y9/l/vi_VN/siofuDX1J2n.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeHL-OE0uJ-CrFOAu_su-jCkFP5ba3RVyCUU_ltrdFXIJfWNm-hiK37pwNLveY6iOEFBl8Lm6j00xb6n0uvgvJr1"
                    },
                    "YLZEJAB": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3iDHA4/yf/l/vi_VN/1Ob5m1l8LUr.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeGu458DxVShF5-Yh8VMdtmnDQrKmVzjCFINCsqZXOMIUjNxAWgVsmLQTxMnEBDtCx9cFpKCRY5DmWp_7gZpjask"
                    },
                    "ak9OmxP": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3icdC4/yC/l/vi_VN/0W22b1CEG1F.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeG684AuUW-FTplyMQ7lI_nuMPk6mZL5N3Ew-TqZkvk3cVHVl77vZDjMTJhR3nU4eA87R7-fFKMtoqHZYQnAmRWp"
                    },
                    "V7lrDtL": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3imDf4/y7/l/vi_VN/jwyz3a46PrJ.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeFyhwNtRq_0bep3dlX4zYbuKpRVMAeeEXgqlFUwB54ReGMKtddbFxzyBqwcNRLO-Z_5sXekzDYJcyDjwGBTBs1u"
                    },
                    "sDwjFDW": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yX/r/4ub-qLkD6cN.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeFoPVm6ddgsQbSqKSqRjcSR8K3TpOwfBJLwrdOk7B8Ekj6jXS7OSyc5K-UR4H6e1DjCgZfUlMHyFhFEgaWL8yeb"
                    },
                    "FcBwX2d": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yc/r/xPB-b6CZl0Q.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeFy1GU14owM5y6sCSyVGu9qNR-FtUAkjE01H4W1QCSMTYxBUhf_1059IXkGCg1EJacigL89dvkiNfCnjcA-eO8w"
                    },
                    "SWx3yNv": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/y7/r/g__eV5OXSXl.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeGFO9QXQguEiWG0FLFi203bJf9rtnptjacl_2u2em2Np6WCMj2hhIcEVBagVK3W9DtyDFx0YFgwRsmUgYTndQ3E"
                    },
                    "WI8qjDr": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3i1G84/yy/l/vi_VN/-eQeNVXKvHz.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeGJaXNIqzjaRMsYN1Dri5FDflqqBaReQJ1-WqoFpF5AnU1FbEqIf14jJ9Z4i8RKdnpjTw098YZ03qMXQNJbLekp"
                    },
                    "oBDkbWt": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3i1Y04/y1/l/vi_VN/yPx79yZRYSk.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeE0-LfaJ2D6I8hWSLO1vPTOz1LgYrf8YvvPUuBit_xi-4D-4YzNkIbJCf73PO_pOAkX1uXySkx-nAxCrooLC1Sh"
                    },
                    "x22Oby4": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yZ/r/tVshp1OIV9l.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeGNjq3MTbIEI2jZF_y-lzmPj4y-a0EbfM-PjL5rQRt8z8wC127YlnuZH_EQd0goeFkSoArHTvZUbVriIPPXFf62"
                    },
                    "8ELCBwH": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/ye/r/VRzSVH5iU-V.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeEzd5h_FsdfMg2jA6mKU-HiB4h8LIzMcEoHiHwsjMxwSjxVVpsLJRwqvyqXHIYSF7lOkxFKrJRFLjkiaJd216o8"
                    },
                    "oE4DofT": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yd/r/i_YUeG5ZtX_.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeHiFQKpWu-Lb8RyRerSRGjDzieZjhaAyW_OJ5mOFoDJb6OkUH8iVvBnn6Fiql4XUh80qMsE6cA6UocFEGhWTFH0"
                    },
                    "I+GHswV": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yS/r/ui2DkP-wt_7.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeFjMQApgjEOgHpRGZNsucu0rXgFt2FOG7KteAW3YU4bsg1kA23C9bpJFkF_uzUYLQWi7bMGGD6AWfHK5pZbnFzx"
                    },
                    "17Grp2h": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/y-/r/HhbMrxvaW_H.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeGgsLNADPZOH49IS_H8KxJUwU2Z5sVeIFDBTZnmxV4gUCVFSMb0OkE5Wz4d0Ap4uteoWikkKGLZ-suZd9fdF_Z6"
                    },
                    "QyoftxH": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yL/r/j-_AFWnS2kv.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeHNNI1Rw-g-pR4bgoYAhZb5twCmduj-KSm3AKZ26P4pKSVkuHva171lmAVKdjLKtW32kuHCwqRhEiI94adzeG8j"
                    },
                    "H/5lfuF": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yF/r/iqrvM8jAXX7.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeGvaYAAPeD8MhXzVH8QuJSSWuoCV9cDZRRa6gJX1wNlFLEpZypJIMnmXlfrRSf3m27zC1dXI7Tgo6AEOsGYumQ7"
                    },
                    "QIamfde": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yA/r/Y37sQzk-yb8.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeGV2091YCYb0P6MbgdStCLqT83xClExge5PzfEKUTGB7qunu3exM2cPhOZ6rnmxQQu7RI7-W_9eEW1F3E9lX0bA"
                    },
                    "geEIDQe": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/ys/r/3IpOtTu97tT.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeGygmgoPR-oIuJgWMStu4zJVaOxW1GrULdVo7FbUatQt-O6Mpy0anCVVr5Qz9meRdkhFU3JNiLhrRJNFFUCq8fh"
                    },
                    "w6++B1W": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yk/r/RKK6hMCj3R1.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeFWJCp-naQZAsRKRwHVuXNdbkLZvsOAZ7huQtm-w4BnuB_XZW8eXYIbrQkskTlGOKT3KSIb10xEcWA36p08Vikl"
                    },
                    "ONXdU/u": {
                        "type": "js",
                        "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/Fas1RmITs0Z.js?_nc_x=z9VIGQBJZK9&_nc_eui2=AeE61UEbXWyC_Xz9s_aPyNE-IR0rKiJ6RrkhHSsqInpGubPkOQ43oBDixxFh5pHTlIjmidT3P-KU4X-aLm0u9w_W"
                    }
                },
                "compMap": {
                    "Dialog": {
                        "r": [
                            "4ICgmNm",
                            "e8KbigC",
                            "BiRHLnG",
                            "d37yUGn",
                            "9bDSwfT",
                            "UmHNvtz",
                            "LVchrHd",
                            "kvx582Y",
                            "3HNSMZt",
                            "Hdg+cXJ",
                            "0TAmMmp",
                            "IYvn1RJ",
                            "qUOfXdB",
                            "bB8N6Cz",
                            "R5w1rCJ",
                            "Ufq6YWX",
                            "Wsv7q+J"
                        ],
                        "rds": {
                            "m": [
                                "FbtLogging",
                                "IntlQtEventFalcoEvent",
                                "Animation",
                                "PageTransitions"
                            ]
                        },
                        "be": 1
                    },
                    "ExceptionDialog": {
                        "r": [
                            "R5w1rCJ",
                            "LbsdIZo",
                            "7+vJC3A",
                            "UHub1Gz",
                            "zaGHrql",
                            "e8KbigC",
                            "rk/b7Sj",
                            "BiRHLnG",
                            "d37yUGn",
                            "UmHNvtz",
                            "LVchrHd",
                            "MJUxMvv",
                            "2IRmU7r",
                            "YLZEJAB",
                            "ak9OmxP",
                            "Wsv7q+J",
                            "kvx582Y",
                            "V7lrDtL",
                            "Hdg+cXJ",
                            "IYvn1RJ",
                            "sDwjFDW",
                            "bB8N6Cz",
                            "FcBwX2d",
                            "qUOfXdB"
                        ],
                        "rds": {
                            "m": [
                                "FbtLogging",
                                "IntlQtEventFalcoEvent"
                            ]
                        },
                        "be": 1
                    },
                    "QuickSandSolver": {
                        "r": [
                            "SWx3yNv",
                            "WI8qjDr",
                            "oBDkbWt",
                            "3HNSMZt",
                            "x22Oby4",
                            "8ELCBwH",
                            "IYvn1RJ",
                            "qUOfXdB",
                            "UmHNvtz"
                        ],
                        "rds": {
                            "m": [
                                "FbtLogging",
                                "IntlQtEventFalcoEvent"
                            ]
                        },
                        "be": 1
                    },
                    "ConfirmationDialog": {
                        "r": [
                            "oE4DofT",
                            "I+GHswV",
                            "d37yUGn",
                            "3HNSMZt",
                            "IYvn1RJ",
                            "UmHNvtz"
                        ],
                        "be": 1
                    },
                    "MWADeveloperReauthBarrier": {
                        "r": [
                            "17Grp2h",
                            "QyoftxH",
                            "H/5lfuF",
                            "QIamfde",
                            "IYvn1RJ"
                        ],
                        "be": 1
                    },
                    "WebSpeedInteractionsTypedLogger": {
                        "r": [
                            "geEIDQe",
                            "IYvn1RJ",
                            "kvx582Y",
                            "w6++B1W"
                        ],
                        "be": 1
                    },
                    "PerfXSharedFields": {
                        "r": [
                            "kvx582Y",
                            "ONXdU/u"
                        ],
                        "be": 1
                    }
                }
            }
        },
        "allResources": [
            "IYvn1RJ",
            "qUOfXdB",
            "UmHNvtz"
        ],
        "lid": "7358018043680021025"
    }
}
```
</details>
