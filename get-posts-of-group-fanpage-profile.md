# APIs-Facebook-no-cookie-token
API lấy data facebook không cần dùng cookie hay token
HOÀN TOÀN MIỄN PHÍ

<details>

<summary>Get full info danh sách bài viết trên fanpage, group, trang cá nhân</summary>

```http
GET http://graph.scanfb.top/graph/v19.0/{ID}/feed?fields=from,id,created_time,message,attachments{media,target,title,type,url,subattachments.limit(100)},comments.summary(total_count).limit(0),reactions.summary(total_count).limit(0),shares&access_token=N8o3eySfREuw1pbt3fmcLg
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `action` | `string` | **Cố định**. Chọn API |
| `{ID}` | `string` | **Bắt buộc**. ID của fanpage/group/profile, dạng số, không có dấu '_' |
| `fields` | `string` |  Các trường thông tin cần lấy, tìm hiểu thêm tại [đây](https://developers.facebook.com/docs/graph-api/) |
| `access_token` | `string` | **Bắt buộc**. Token trên được chia sẽ công khai, nhiều người dùng, request có thể sẽ chậm. Liên hệ Kiệt để nhận Token riêng miễn phí |


### Response
```json
{
    "success": true,
    "message": "",
    "data": {
        "data": [
            {
                "id": "1777766135578951_7527887927233381",
                "created_time": "2024-04-13T22:58:49+07:00",
                "message": "Cần tìm bác nào có kinh nghiệm build core trình duyệt ạ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 4
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                }
            },
            {
                "id": "1777766135578951_7533949509960556",
                "created_time": "2024-04-15T10:39:28+07:00",
                "message": "Chạy file python trong c# sử dụng class Process, lấy output text, ai làm được inbox mình, ngân sách 500k. Ai làm được cho mình xem demo, ok thì mình bank liền. Lấy được cái đoạn \"please enter ...\", rồi nhập được 1 số phone bất kỳ là ok. Yêu cầu ko dùng ocr, ko tắt python.\nSource file login.py như sau:\nfrom telethon import TelegramClient, events, sync\napi_id = 1100092\napi_hash = '156e4934a45aca5b9c39e72056d80f2a'\n\nclient = TelegramClient(\"d:\\\\661c9cb297184644345885c1.json\", api_id, api_hash)\nclient.start()",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 100,
                                    "src": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.30808-6/437859782_8307632555919529_7762491747549246741_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeH4VSJfXzD5JdvxnRUcwBaYjOJVU3eCx2iM4lVTd4LHaOKZNAGTJE6OjLTDKQLKdDqy6vr1ym5BDbfImXswWs1G&_nc_ohc=BP7EhPYUbaYAb5PEAHV&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfDW7I7NWxrApjQ4z6As9kjEAMqrhJKuC5Yq1RLppAOxcQ&oe=6622CB4F",
                                    "width": 1350
                                }
                            },
                            "target": {
                                "id": "8307632565919528",
                                "url": "https://www.facebook.com/photo.php?fbid=8307632565919528&set=gm.7533949509960556&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=8307632565919528&set=gm.7533949509960556&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 8
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 5
                    }
                }
            },
            {
                "id": "1777766135578951_7517487571606750",
                "created_time": "2024-04-11T14:35:07+07:00",
                "message": "Cần thầy dạy auto trình duyệt phục vụ làm mmo\nThầy nào dạy uy tín ae giới thiêụ giúp mình với",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 13
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 22
                    }
                }
            },
            {
                "id": "1777766135578951_7533350010020506",
                "created_time": "2024-04-15T06:54:50+07:00",
                "message": "Cần Mua code python nhắn tin zalo = request, ai có inbox mình nhé.",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 2
                    }
                }
            },
            {
                "id": "1777766135578951_7523377607684413",
                "created_time": "2024-04-12T22:23:32+07:00",
                "message": "Share nguồn facebook graph API miễn phí.\nCó thể quét được gần như tất cả dữ liệu facebook : \n* Tất cả bài viết trên một fanpage, trang cá nhân, nhóm công khai\n* Tất cả bình luận của một bài viết\n* Tất cả video của fanpage, group, trang cá nhân\n* ...\n\nNếu các bác chưa biết dùng graph api nhưng có nhu cầu cào dữ liệu gì của facebook thì cứ inbox em hướng dẫn nha\n\nHướng dẫn : dành cho người đã biết dùng facebook graph api\n1. Thay domain 'https://graph,facebook,com' bằng 'http://graph,scanfb,top/graph'\n1. Thay access_token bằng access_token của bên em\n1. Gọi API và nhận kết quả",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 720,
                                    "src": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.30808-6/435068514_1575427643304330_3767916661727619302_n.jpg?stp=dst-jpg_p720x720&_nc_cat=101&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeGdAqJITCDkj3Hz3P9DoyVRk4wOiSqvBaqTjA6JKq8FqvRxXoT4IikQaEKEpaJHmOUBs5cOGNfBoG_LLj2o0wYx&_nc_ohc=lzSEZM8lHgUAb7xto_2&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfBtzQ__4JuGWp8fKMB7nWeJJp9PJDk-I-Ym3Pztw_iLnA&oe=6622B65F",
                                    "width": 994
                                }
                            },
                            "target": {
                                "id": "1575427646637663",
                                "url": "https://www.facebook.com/photo.php?fbid=1575427646637663&set=gm.7523377607684413&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=1575427646637663&set=gm.7523377607684413&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 7
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 35
                    }
                },
                "shares": {
                    "count": 5
                }
            },
            {
                "id": "1777766135578951_7530150857007088",
                "created_time": "2024-04-14T12:43:54+07:00",
                "message": "Các bác cho em hỏi là có cách nào để check trạng thái LDPLayer đã khởi động xong\nhoặc mở 1 app đã khởi động xong chưa không ạ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 7
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7530005820354925",
                "created_time": "2024-04-14T11:49:21+07:00",
                "message": "E cần tìm bác nào có kinh nghiệm build core trình duyệt chromium ạ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 12
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 5
                    }
                }
            },
            {
                "id": "1777766135578951_7533872293301611",
                "created_time": "2024-04-15T10:11:04+07:00",
                "message": "Cần người viết tool tạo gmail live 30p mà không xác minh sđt, ae nào có xin giá vào inbox nhé.",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 8
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 13
                    }
                }
            },
            {
                "id": "1777766135578951_7533978109957696",
                "created_time": "2024-04-15T10:50:21+07:00",
                "message": "Em chào các bác, e có vọc vạch chút ở gologin nhưng đang gặp vấn đề ở chỗ profile trong gologin thì ngon lành nhưng khi download về và chạy với selenium (chromedriver) thì nó đang không ăn khớp các thông số. E có check các thông số bên trong file json thì vẫn đúng, có thể là do orbita browser đang gặp vấn đề. Có bác nào bị thế không ạ, có cao kiến gì không ạ?\n\nTài khoản offline:\n* https://ctrlv.link/NSgo\n* https://ctrlv.link/Mub2\n\nTài khoản trên gologin:\n* https://ctrlv.link/qmiW\n* https://ctrlv.link/qqLt",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 720,
                                    "src": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.30808-6/437944324_2244770452535890_4704250853574785175_n.jpg?stp=dst-jpg_p720x720&_nc_cat=109&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEfDE7ffibZnPKaRQVyOlF-LqHszu9WMxouoezO71YzGsmFMywAHsOZNAkqHc6EbULhcDnNy8tkUavmtGU53SL5&_nc_ohc=1qHpxUTciy4Ab5irMXb&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfDRpNM03l4bygvSDFtXuWQL7SQR3fAK-hmXFqvSZDNfhA&oe=6622A27A",
                                    "width": 1355
                                }
                            },
                            "target": {
                                "id": "7533978109957696",
                                "url": "https://www.facebook.com/media/set/?set=pcb.7533978109957696&type=1"
                            },
                            "title": "Ảnh từ bài viết của Tuấn",
                            "type": "album",
                            "url": "https://www.facebook.com/media/set/?set=pcb.7533978109957696&type=1",
                            "subattachments": {
                                "data": [
                                    {
                                        "media": {
                                            "image": {
                                                "height": 720,
                                                "src": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.30808-6/437944324_2244770452535890_4704250853574785175_n.jpg?stp=dst-jpg_p720x720&_nc_cat=109&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEfDE7ffibZnPKaRQVyOlF-LqHszu9WMxouoezO71YzGsmFMywAHsOZNAkqHc6EbULhcDnNy8tkUavmtGU53SL5&_nc_ohc=1qHpxUTciy4Ab5irMXb&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfDRpNM03l4bygvSDFtXuWQL7SQR3fAK-hmXFqvSZDNfhA&oe=6622A27A",
                                                "width": 1355
                                            }
                                        },
                                        "target": {
                                            "id": "2244770455869223",
                                            "url": "https://www.facebook.com/photo.php?fbid=2244770455869223&set=gm.7533978103291030&type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/photo.php?fbid=2244770455869223&set=gm.7533978103291030&type=3"
                                    },
                                    {
                                        "media": {
                                            "image": {
                                                "height": 441,
                                                "src": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.30808-6/438206111_2244771209202481_4094802918706858928_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHpcGZ1lwuO_G56Gf-P1KL_5ylQ-qDIGJnnKVD6oMgYmV4NhHHlQLCKz10blztn06WiHIsInZhd3uU9P2eC-GsI&_nc_ohc=muRgpC1D8ocAb6j8X5L&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfBhTOchx7WP0gBM2DuFsXHIi4_Flnxk6G34-ZpFjNkWOg&oe=6622C94E",
                                                "width": 1438
                                            }
                                        },
                                        "target": {
                                            "id": "2244771212535814",
                                            "url": "https://www.facebook.com/photo.php?fbid=2244771212535814&set=gm.7533978106624363&type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/photo.php?fbid=2244771212535814&set=gm.7533978106624363&type=3"
                                    }
                                ]
                            }
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                }
            },
            {
                "id": "1777766135578951_7479386825416825",
                "created_time": "2024-04-02T15:08:19+07:00",
                "message": "**Thuật toán mã hóa dữ liệu khi requests bằng XOR #2**\n\nRảnh mình ngồi nghịch api của thằng tiktok thì mới thấy cái api cũ của nó , dùng thuật toán này để mã hóa user , password , email , ..\n\nLúc đầu mình nghĩ nó là md5 nhưng check cái hash của email mới thấy ra 40  có lúc lại nhỏ hơn 40\n\nmà theo như mình biết thì md5 nó là 32 kí tự\n\nsau đó check lại cái mật khẩu thì thấy mật khẩu ngắn cho ra đoạn mã ngắn - mật khẩu dài cho ra đoạn mã hóa dài.\n\nTừ đó mình loại bỏ được cái này không phải md5 -> cũng chả phải hex , hay sha\n\nTiếp sau đó mình cố tình để mật khẩu có các kí tự giống nhau ( không để ở email được vì email dài và để thiếu dấu @ thì không hợp lệ)\n\nsau khi test ở mật khẩu để kí tự aaa => chuỗi hash trả về là 646464 bất ngờ là ở chỗ này. Mình nhận ra thằng này kí tự sau khi mã hóa\n\ntrả về giống nhau cho các kí tự với kí tự a được mã hóa bằng 64\n\nvà nhiều kí tự a thì vẫn cứ là 64646464 mình đoán nó là XOR\n\n**Nhưng cái đang gặp phải ở đây là :V làm sao để biết được key của thuật toán xor trong khi biết giá trị đầu vào và đầu cuối ngoài cách xem soure app**\n\n- post  tương tự về mã hóa dữ liệu xor từ đó dịch ngược để lấy ra email protected\n\n=> https://www.facebook.com/groups/autocsharp/posts/7380937995261709/",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 65,
                                    "src": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-6/430882466_1386225886108520_3300569125967686009_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHME9h2euStgPBZDQsHme7WqsR22Pq-qIyqxHbY-r6ojFDN6QX9G9BSbjNe6uVXBkRghg_3SiiAfuRvR33TW2Uv&_nc_ohc=z-1POmKzBjUAb4t1Q1-&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfAOcym05BjXftlpef6o0EBSUu9aZzL9gLZnir_0j84wYQ&oe=6622BEEE",
                                    "width": 530
                                }
                            },
                            "target": {
                                "id": "7380937995261709",
                                "url": "https://www.facebook.com/media/set/?set=pcb.7380937995261709&type=1"
                            },
                            "title": "Ảnh từ bài viết của Nguyen Van Hung",
                            "type": "album",
                            "url": "https://www.facebook.com/media/set/?set=pcb.7380937995261709&type=1",
                            "subattachments": {
                                "data": [
                                    {
                                        "media": {
                                            "image": {
                                                "height": 65,
                                                "src": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-6/430882466_1386225886108520_3300569125967686009_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHME9h2euStgPBZDQsHme7WqsR22Pq-qIyqxHbY-r6ojFDN6QX9G9BSbjNe6uVXBkRghg_3SiiAfuRvR33TW2Uv&_nc_ohc=z-1POmKzBjUAb4t1Q1-&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfAOcym05BjXftlpef6o0EBSUu9aZzL9gLZnir_0j84wYQ&oe=6622BEEE",
                                                "width": 530
                                            }
                                        },
                                        "target": {
                                            "id": "1386225892775186",
                                            "url": "https://www.facebook.com/photo.php?fbid=1386225892775186&set=gm.7380937988595043&type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/photo.php?fbid=1386225892775186&set=gm.7380937988595043&type=3"
                                    },
                                    {
                                        "media": {
                                            "image": {
                                                "height": 60,
                                                "src": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-6/431360237_1386226669441775_1209087339080396646_n.jpg?_nc_cat=103&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHTFqi9R0Z1iPoBbRjef7EM5UCTlVYoZjXlQJOVVihmNYPvj3SrLdNRlPhnb9NiCn040vUhHBfJ-NpoViz_t_Qs&_nc_ohc=AYtU7_-WcyUAb71qDui&_nc_oc=AdibnMAtufDU3GzWh7wC35tcYaGAhHvurKDup3uenzaM4sD9vXXbRdGmzncenPqF9TY&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfASSl5ei7uIkE9CmXuCf6pYEn0yRhrVJ3lTDAUJ2t2xWQ&oe=6622C65F",
                                                "width": 359
                                            }
                                        },
                                        "target": {
                                            "id": "1386226676108441",
                                            "url": "https://www.facebook.com/photo.php?fbid=1386226676108441&set=gm.7380937991928376&type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/photo.php?fbid=1386226676108441&set=gm.7380937991928376&type=3"
                                    }
                                ]
                            }
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 8
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 69
                    }
                },
                "shares": {
                    "count": 11
                }
            },
            {
                "id": "1777766135578951_7534045006617673",
                "created_time": "2024-04-15T11:16:18+07:00",
                "message": "Lập trình hỗ trợ được rất nhiều thứ trong cuộc sống. Series chia sẽ này tập trung nói về khả năng ứng dụng của lập trình. Mọi ngươi nhớ like, flow và share để không bõ lỡ bài mới nhé.",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 720,
                                    "src": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.30808-6/434710122_7325821144205760_8871569717688023392_n.jpg?stp=dst-jpg_p720x720&_nc_cat=108&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeFDSY8_iFNrDV3lDNBnIZL-UOrcLxswWq1Q6twvGzBarXGFV1kYkQob5MvjgSa3-XEq3PUXzbqeQqVg5c85UtNo&_nc_ohc=XY_ifPlte0EAb5dlpRH&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfBUB6W-80Cgsg2xtCZf7Kan-E-T6H2Bl1echV2d_IaDNg&oe=6622BF3F",
                                    "width": 1280
                                }
                            },
                            "target": {
                                "id": "7325821147539093",
                                "url": "https://www.facebook.com/photo.php?fbid=7325821147539093&set=a.243373215783957&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=7325821147539093&set=a.243373215783957&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 9
                    }
                }
            },
            {
                "id": "1777766135578951_7530611690294338",
                "created_time": "2024-04-14T15:30:46+07:00",
                "message": "Template code cho bạn nào dùng C#\n",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 720,
                                    "src": "https://external.fsgn2-11.fna.fbcdn.net/emg1/v/t13/4313046682556219414?url=https%3A%2F%2Fi.ytimg.com%2Fvi%2FvYYVLldxp5I%2Fmaxresdefault.jpg%3Fsqp%3D-oaymwEmCIAKENAF8quKqQMa8AEB-AH-CYAC0AWKAgwIABABGGUgZShlMA8%3D%26rs%3DAOn4CLBEwjmdR3Th0dubycj5Eb24ILqRjw&fb_obo=1&utld=ytimg.com&stp=c0.5000x0.5000f_dst-emg0_p720x720_q75&_nc_eui2=AeHyd9SwSEAAU3-rhOxDXT0wxV7upgkH22rFXu6mCQfbakW74iP1hZhbYGWxB_35Hm7Szyh8Y46B4Vr6VicTH2Bh&ccb=13-1&oh=06_Q3992-TLCQZ1IA1L7ykwpNJgmIOM-sFA83hDi5b0VOvgwww&oe=661EDC30&_nc_sid=ef6713",
                                    "width": 720
                                },
                                "source": "https://www.youtube.com/embed/vYYVLldxp5I?autoplay=1"
                            },
                            "target": {
                                "url": "https://l.facebook.com/l.php?u=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DvYYVLldxp5I&h=AT3UJyfrPFRaOQbwNETWBrZ79KVX9uffcrbuoSvHQnt726uam1Xvmzrm5uuz_Z--dKBGJU81kN-xWZ7eEoOZidt41KlmRdyLu55mlokYLPsaRbcJPTh6nO8kW5dlnew6kmcdIEfRvLg&s=1"
                            },
                            "title": "Undetected Chromedriver C# Selenium Multilple threading Template",
                            "type": "share",
                            "url": "https://l.facebook.com/l.php?u=https%3A%2F%2Fwww.youtube.com%2Fwatch%3Fv%3DvYYVLldxp5I&h=AT3UJyfrPFRaOQbwNETWBrZ79KVX9uffcrbuoSvHQnt726uam1Xvmzrm5uuz_Z--dKBGJU81kN-xWZ7eEoOZidt41KlmRdyLu55mlokYLPsaRbcJPTh6nO8kW5dlnew6kmcdIEfRvLg&s=1"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 49
                    }
                },
                "shares": {
                    "count": 20
                }
            },
            {
                "id": "1777766135578951_7533699313318909",
                "created_time": "2024-04-15T09:07:07+07:00",
                "message": "làng nước ơi   embanvia. com  cam kết  bán   nguyên liệu  rẻ nhất thị trường -  Chỗ nào   bán  rẻ chúng tôi bán rẻ hơn -  Ở đâu  uy tín chúng tôi uy tín hơn",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 720,
                                    "src": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-6/437755688_1469749140564991_839440596628023760_n.jpg?stp=dst-jpg_p720x720&_nc_cat=106&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHt5Yb9JQs5adjq08KMiUP9G8Kho6y1UIobwqGjrLVQimnyLV55kv_j38WQQAYHuYtHr1bTCScLJfSUCfOTptc3&_nc_ohc=6MAYHfgOcVYAb6Z0SYk&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfAqMkzxmK-POPEmsmgEOVbihrtpAvl9orN2n6gbrlsKhQ&oe=6622AB9A",
                                    "width": 720
                                }
                            },
                            "target": {
                                "id": "1469749143898324",
                                "url": "https://www.facebook.com/photo.php?fbid=1469749143898324&set=gm.7533699313318909&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=1469749143898324&set=gm.7533699313318909&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                }
            },
            {
                "id": "1777766135578951_7531506760204831",
                "created_time": "2024-04-14T20:28:19+07:00",
                "message": "Mọi người cho mình hỏi mình có chơi game trên Web, muốn khi có một nút hiện lên thì click vào, đa luồng và không chiếm chuột thì phần mềm AMK có làm được không, cảm ơn mọi người\n.",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7522608504427990",
                "created_time": "2024-04-12T18:36:07+07:00",
                "message": "Em cần mua api lấy khoá luồng Livestream tiktok và api ping live đó live được 24/24",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 5
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 5
                    }
                }
            },
            {
                "id": "1777766135578951_7521389754549865",
                "created_time": "2024-04-12T11:41:17+07:00",
                "message": "Mấy bác cho em hỏi đoạn Selenium này với ạ. Khi em nhập sđt báo lỗi e nhập lại số khác. Trước khi nhập số khác em cần xóa số củ đi. Nhưng em thử đủ cách. Clear() và Send key cũng không xóa được ạ. :(",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 372,
                                    "src": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.30808-6/438030235_2419671851564223_1718245601332523067_n.jpg?_nc_cat=102&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHUVmfvf0cvsGi2nyaSyLXr_qjm5XBuBjb-qOblcG4GNiuiJpP7EbLToBlZHIzDmsbOqpj5h0OVHWPh85955FjH&_nc_ohc=wB9I1eIPxt4Ab45x4rV&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfAZGTVCATqA5SSst8bLFEldEyuaJFUyQyDDMUB9i8Jllg&oe=6622A111",
                                    "width": 1368
                                }
                            },
                            "target": {
                                "id": "2419671854897556",
                                "url": "https://www.facebook.com/photo.php?fbid=2419671854897556&set=gm.7521389754549865&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=2419671854897556&set=gm.7521389754549865&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 10
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 9
                    }
                }
            },
            {
                "id": "1777766135578951_7521907034498137",
                "created_time": "2024-04-12T14:41:35+07:00",
                "message": "Cần 1 bạn viết extension chrome đăng reel facebook.\nBạn nào ở HN thì giao dịch trực tiếp, còn nơi khác thì trung gian\ntks all",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 960,
                                    "src": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.30808-6/435712306_393130677017763_4351264979900226318_n.jpg?stp=dst-jpg_p720x720&_nc_cat=105&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEzloUD5WJSR6iJDEuq0ty_mEbxzQsCbriYRvHNCwJuuI1qAwKPupY4OTrdbFcZ-nZ2X4HxKM1QxlNAQWS_R5H6&_nc_ohc=kW35310HgpwAb6j4yNx&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfC9kFLhgOMTt3PKiK6zd8frShAOuJUob1uA0grnnqPeEg&oe=6622B1B0",
                                    "width": 720
                                }
                            },
                            "target": {
                                "id": "393130687017762",
                                "url": "https://www.facebook.com/photo.php?fbid=393130687017762&set=gm.7521907034498137&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=393130687017762&set=gm.7521907034498137&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 4
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 7
                    }
                }
            },
            {
                "id": "1777766135578951_7526340464054794",
                "created_time": "2024-04-13T14:37:56+07:00",
                "message": "tìm tool tạo gmail live 30p. (hoặc site bật sẵn imap) Ai có ib em với ạ.",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 7
                    }
                }
            },
            {
                "id": "1777766135578951_7529607487061425",
                "created_time": "2024-04-14T09:20:25+07:00",
                "message": "1. [Puppeteer](https://github.com/chenrensong/PuppeteerAot) sharp tương thích aot cho bác nào thích, dung lượng sẽ nhỏ hơn selenium dùng NewtonSoft.Json tầm 10mb https://github.com/chenrensong/PuppeteerAot",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 600,
                                    "src": "https://external.fsgn2-11.fna.fbcdn.net/emg1/v/t13/17309571605257454875?url=https%3A%2F%2Fopengraph.githubassets.com%2Fb5aa3d35e2e7de5a917a20c3ffb35ccaef2160197da148e4463546bbfb98317b%2Fchenrensong%2FPuppeteerAot&fb_obo=1&utld=githubassets.com&stp=c0.5000x0.5000f_dst-emg0_p600x600_q75&_nc_eui2=AeE9nUxxN8T_tIwuAXmi5AyUcOSNrpWRp09w5I2ulZGnT-7nzyWxtpHteRSDQDS7VVHIWkLQEnIjom0DOtTFObFW&ccb=13-1&oh=06_Q399kgoifhCN7pRbDvtk49nzV1vYffkvE4HOTtdRuWjk0Y8&oe=661EE173&_nc_sid=ef6713",
                                    "width": 600
                                }
                            },
                            "target": {
                                "url": "https://l.facebook.com/l.php?u=https%3A%2F%2Fgithub.com%2Fchenrensong%2FPuppeteerAot&h=AT2khJ5T137uUVFdt4lZdFleoR7LU5vU7DKsI2Y4OrQn69XO3e3ep3GAbeEnaVmlOZytEjYm2ktGiPpsQsiTJu9t_pMYbqQvxg7E_1W72WWYZCSONjp8IKjx43DMk01aDVgROUB2OkM&s=1"
                            },
                            "title": "GitHub - chenrensong/PuppeteerAot: Headless Chrome .NET API and support for AOT compilation",
                            "type": "share",
                            "url": "https://l.facebook.com/l.php?u=https%3A%2F%2Fgithub.com%2Fchenrensong%2FPuppeteerAot&h=AT2khJ5T137uUVFdt4lZdFleoR7LU5vU7DKsI2Y4OrQn69XO3e3ep3GAbeEnaVmlOZytEjYm2ktGiPpsQsiTJu9t_pMYbqQvxg7E_1W72WWYZCSONjp8IKjx43DMk01aDVgROUB2OkM&s=1"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 4
                    }
                }
            },
            {
                "id": "1777766135578951_7532261803462660",
                "created_time": "2024-04-15T00:16:25+07:00",
                "message": "Xin phép admin và các bác ạ.\nEm cần mua giải pháp giải captcha này ạ. \nCode demo C# vs Cefsharp ạ.",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 435,
                                    "src": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.30808-6/438030023_399866002817383_7570996265051224329_n.png?_nc_cat=108&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeE_k_eCLIBNL-3bP_-NJabvwKRfFnqTX-bApF8WepNf5hcH3HtAZiPJeaxH7dcTTucR_c7HqRlWXAgXJptpbmf7&_nc_ohc=k8tJhmofRYIAb44Byp9&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfCqJEUMS7QVA0nm_R7SCVZJowm_xvQB0aekGM8QHYFZkQ&oe=6622AE11",
                                    "width": 513
                                }
                            },
                            "target": {
                                "id": "399866006150716",
                                "url": "https://www.facebook.com/321076107363040/photos/gm.7532261803462660/399866006150716/?type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/321076107363040/photos/gm.7532261803462660/399866006150716/?type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7531520100203497",
                "created_time": "2024-04-14T20:32:18+07:00",
                "message": "Mọi người cho em hỏi , e muốn chạy đa luồng trên gologin bằng bằng package pyautogui có được ko ạ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                }
            },
            {
                "id": "1777766135578951_7527000707322103",
                "created_time": "2024-04-13T18:29:41+07:00",
                "message": "Giờ google không cho gửi mail bằng smtp vs pass ứng dụng nữa rồi, giờ còn cách nào để setup gửi mail ko các bác",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7530630586959115",
                "created_time": "2024-04-14T15:38:03+07:00",
                "message": "làng nước ơi   embanvia , com  cam kết  cung cấp   nguyên liệu  rẻ nhất thị trường -  Chỗ nào   cung cấp  rẻ chúng tôi bán rẻ hơn -  Chỗ nào  uy tín chúng tôi uy tín hơn",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 720,
                                    "src": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.30808-6/435927310_1469320540607851_3693974778924044645_n.jpg?stp=dst-jpg_p720x720&_nc_cat=108&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeGsL-9ghCBG-oj1-og9VivIhLilbUjlt-yEuKVtSOW37Jr3EXlNdPf9bWhnKxGlC6EorrzzWJIEmh5q7viePWNC&_nc_ohc=dS1prL0O7p8Ab6WrzLa&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfCrTvpl_UHSIb2N95bdRfVXpFGoiqVeeREJvs5-BPu1yw&oe=6622D22E",
                                    "width": 720
                                }
                            },
                            "target": {
                                "id": "1469320543941184",
                                "url": "https://www.facebook.com/photo.php?fbid=1469320543941184&set=gm.7530630586959115&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=1469320543941184&set=gm.7530630586959115&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                }
            },
            {
                "id": "1777766135578951_7530513146970859",
                "created_time": "2024-04-14T14:55:10+07:00",
                "message": "Mình cần học về request và web3 để làm auto. Có thầy nào dạy k ạ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 2
                    }
                }
            },
            {
                "id": "1777766135578951_7530074710348036",
                "created_time": "2024-04-14T12:16:00+07:00",
                "message": "Em newbie có viết tool Reg Twitter chạy Full Request phục vụ mục đích cá nhân. Em cần bán lại source code cho bác nào vọc . Do viết bằng python nên khó thương mại. \n-Reg twitter và Unlock Twitter \n-Auto solve captcha by Rockcaptcha\nBác nào mua source về để vọc thì inbox em ạ! Em cảm ơn\nTele: @jonyssk cho dễ nói chuyện ạ",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 405,
                                    "src": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t15.5256-10/421071690_1147189360067952_2574350043570914242_n.jpg?stp=dst-jpg_s720x720&_nc_cat=110&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeG5CMXByDv8h_7NQO6teVEZ3MHuKpqvBXPcwe4qmq8Fc4V3jxL0mplcIZHllRfPSfIBL96DhtztrQ1piCLGut7u&_nc_ohc=Dq4-VmP4-moAb58MMRA&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfBEeaEQ5u7kb79N2Yy1cGy4MlNctoqfYrr6DzQyadqpqA&oe=6622CDD7",
                                    "width": 720
                                },
                                "source": "https://scontent.fsgn2-11.fna.fbcdn.net/o1/v/t2/f1/m69/GP-pDBpiZGwhoXMDAOpi3gGQ_21CbmdjAAAF.mp4?efg=eyJ2ZW5jb2RlX3RhZyI6Im9lcF9oZCJ9&_nc_ht=scontent.fsgn2-11.fna.fbcdn.net&_nc_cat=102&_nc_eui2=AeHRSA8ZEmJx1lfcpqRAhMLJFNQz-PW8RCEU1DP49bxEIf2rbf-qUy5kj6cWaX1HTiZX8_0Oac2VORjhK8ijAO3e&strext=1&vs=fa70d8e25c4f90c&_nc_vs=HBksFQIYOnBhc3N0aHJvdWdoX2V2ZXJzdG9yZS9HUC1wREJwaVpHd2hvWE1EQU9waTNnR1FfMjFDYm1kakFBQUYVAALIAQAVAhg6cGFzc3Rocm91Z2hfZXZlcnN0b3JlL0dGbDFEUnJLMEJRazRhTUhBSW9kSG1LdWFQVkpidjRHQUFBRhUCAsgBAEsHiBJwcm9ncmVzc2l2ZV9yZWNpcGUBMQ1zdWJzYW1wbGVfZnBzABB2bWFmX2VuYWJsZV9uc3ViACBtZWFzdXJlX29yaWdpbmFsX3Jlc29sdXRpb25fc3NpbQAoY29tcHV0ZV9zc2ltX29ubHlfYXRfb3JpZ2luYWxfcmVzb2x1dGlvbgAddXNlX2xhbmN6b3NfZm9yX3ZxbV91cHNjYWxpbmcAEWRpc2FibGVfcG9zdF9wdnFzABUAJQAcjBdAAAAAAAAAABERAAAAJsz1y7vwl6sGFQIoAkMzGAt2dHNfcHJldmlldxwXQGTCp%2B%2Bdsi0YIWRhc2hfZ2VuMmh3YmFzaWNfaHEyX2ZyYWdfMl92aWRlbxIAGBh2aWRlb3MudnRzLmNhbGxiYWNrLnByb2Q4ElZJREVPX1ZJRVdfUkVRVUVTVBsKiBVvZW1fdGFyZ2V0X2VuY29kZV90YWcGb2VwX2hkE29lbV9yZXF1ZXN0X3RpbWVfbXMBMAxvZW1fY2ZnX3J1bGUHdW5tdXRlZBNvZW1fcm9pX3JlYWNoX2NvdW50BTI5OTA3EW9lbV9pc19leHBlcmltZW50AAxvZW1fdmlkZW9faWQPODE1MjIyODkwNTM5OTU4Em9lbV92aWRlb19hc3NldF9pZA8zOTk5NTU1OTI4MTI4MzMVb2VtX3ZpZGVvX3Jlc291cmNlX2lkEDE3ODM4MTgwOTIxMTczNTAcb2VtX3NvdXJjZV92aWRlb19lbmNvZGluZ19pZA85NzE4MDgwMzcyMDgxMzIOdnRzX3JlcXVlc3RfaWQAJQIcACXEARsHiAFzBDk0NTkCY2QKMjAyNC0wNC0xMwNyY2IFMjk5MDADYXBwBVZpZGVvAmN0CkdST1VQX1BPU1QTb3JpZ2luYWxfZHVyYXRpb25fcwoxNjYuMDgzMzMzAnRzFXByb2dyZXNzaXZlX2VuY29kaW5ncwA%3D&ccb=9-4&oh=00_AfAiUhShOWHl1FNuBy4xjhbNhAxAjRSRsh2etoVKmA5AUA&oe=661ECB50&_nc_sid=1d576d&_nc_rid=642688182510352&_nc_store_type=1"
                            },
                            "target": {
                                "id": "815222890539958",
                                "url": "https://www.facebook.com/groups/autocsharp/permalink/7530074710348036/"
                            },
                            "type": "video_autoplay",
                            "url": "https://www.facebook.com/groups/autocsharp/permalink/7530074710348036/"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 15
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 61
                    }
                },
                "shares": {
                    "count": 1
                }
            },
            {
                "id": "1777766135578951_7530317306990443",
                "created_time": "2024-04-14T13:44:31+07:00",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 501,
                                    "src": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-6/437671777_813893967456810_9031556968007518475_n.jpg?_nc_cat=103&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeG695wUowaDjNouApb0NDyV1YfvbktkVKDVh-9uS2RUoOZIY-EUiGXgd5OXG8foHlOoTJLht2JfWkEy0qdI4JJA&_nc_ohc=LUWUhZHLarkAb5LCLiH&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfAmAp5V2sGa3naP3x4NNJ69EZfR5Z2Q7nhMDf_IkUl8Ag&oe=6622CD87",
                                    "width": 851
                                }
                            },
                            "target": {
                                "id": "813893970790143",
                                "url": "https://www.facebook.com/photo.php?fbid=813893970790143&set=a.449583293887881&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=813893970790143&set=a.449583293887881&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                }
            },
            {
                "id": "1777766135578951_7525847890770718",
                "created_time": "2024-04-13T11:45:14+07:00",
                "message": "Các bác cho em hỏi. Em bị mắc đoạn nhúng ld vào panel. Nhúng ok r nhưng ld mở xong bị cút chỗ nào ko bt lun ạ 🤡. Thanks ạ",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 568,
                                    "src": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-6/436043444_122132061320222326_2863328558084630836_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeGW1bdIqCZBwm-HgWXmRT0EKTQnPk1XeWIpNCc-TVd5Yg4JIPwBFao59lg9PdbyKMsdWAOrmGJZYggGWtHv3Cj0&_nc_ohc=qU_KNn-t1HgAb48FQcC&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfCrhn8E_YKetYPHkXVI-b_UJoaUrMOtR5iDO00dIAO5gw&oe=6622B3F4",
                                    "width": 734
                                }
                            },
                            "target": {
                                "id": "7525847890770718",
                                "url": "https://www.facebook.com/media/set/?set=pcb.7525847890770718&type=1"
                            },
                            "title": "Ảnh từ bài viết của Anh Nguyen",
                            "type": "album",
                            "url": "https://www.facebook.com/media/set/?set=pcb.7525847890770718&type=1",
                            "subattachments": {
                                "data": [
                                    {
                                        "media": {
                                            "image": {
                                                "height": 568,
                                                "src": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-6/436043444_122132061320222326_2863328558084630836_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeGW1bdIqCZBwm-HgWXmRT0EKTQnPk1XeWIpNCc-TVd5Yg4JIPwBFao59lg9PdbyKMsdWAOrmGJZYggGWtHv3Cj0&_nc_ohc=qU_KNn-t1HgAb48FQcC&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfCrhn8E_YKetYPHkXVI-b_UJoaUrMOtR5iDO00dIAO5gw&oe=6622B3F4",
                                                "width": 734
                                            }
                                        },
                                        "target": {
                                            "id": "122132061326222326",
                                            "url": "https://www.facebook.com/photo.php?fbid=122132061326222326&set=gm.7525847884104052&type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/photo.php?fbid=122132061326222326&set=gm.7525847884104052&type=3"
                                    },
                                    {
                                        "media": {
                                            "image": {
                                                "height": 570,
                                                "src": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-6/435720296_122132061686222326_2492270552488283898_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHBog38kVXLMbogQsCes647NBPkeRuovzc0E-R5G6i_N_CkItw8qYqstxvnCIPvLa1qJ0KqFNokzSMWSV9W-ASN&_nc_ohc=QfHIb6fhHggAb6dE8vd&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfCh1v_bB9r51w-CnwkAI7c9sydBZDRSSA-vopgkOnPRqA&oe=6622CF54",
                                                "width": 831
                                            }
                                        },
                                        "target": {
                                            "id": "122132061692222326",
                                            "url": "https://www.facebook.com/photo.php?fbid=122132061692222326&set=gm.7525847887437385&type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/photo.php?fbid=122132061692222326&set=gm.7525847887437385&type=3"
                                    }
                                ]
                            }
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 4
                    }
                }
            },
            {
                "id": "1777766135578951_7527971923891648",
                "created_time": "2024-04-13T23:24:01+07:00",
                "message": "Em đang gặp lỗi không chụp được ảnh không biết tại sao bác nào giúp e với ạ",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 720,
                                    "src": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.30808-6/436373096_3544143119234740_2608403435044659746_n.jpg?stp=dst-jpg_p720x720&_nc_cat=105&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeFmjgUz0rKKc9NR_AoGwAjfGrN5gBlnv0was3mAGWe_TMKKVJuPkyA5I4KEBF7MqkvxfM77DZSx6LqHttxoQY8Y&_nc_ohc=2ykQzCT_YNQAb4CiY0z&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfCz9GpV412tZ-VmDB04IZ6ovqNe76zmnY94Zs17Ezc9-w&oe=6622B81F",
                                    "width": 1357
                                }
                            },
                            "target": {
                                "id": "3544143122568073",
                                "url": "https://www.facebook.com/photo.php?fbid=3544143122568073&set=gm.7527971923891648&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=3544143122568073&set=gm.7527971923891648&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 2
                    }
                }
            },
            {
                "id": "1777766135578951_7514939711861536",
                "created_time": "2024-04-10T23:58:03+07:00",
                "message": "Có bác nào đang encryted pwd fb bằng cách này k \nhttps://gist.github.com/huoshan12345/44b1b4927b21d4ec21d1cbd61ea659da\nCòn hoạt động k các bác",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 640,
                                    "src": "https://external.fsgn2-11.fna.fbcdn.net/emg1/v/t13/9887746703658296778?url=https%3A%2F%2Fgithub.githubassets.com%2Fassets%2Fgist-og-image-54fd7dc0713e.png&fb_obo=1&utld=githubassets.com&stp=c0.5000x0.5000f_dst-emg0_p640x640_q75&_nc_eui2=AeFEhGgpCYt1oDRttPCdXe2p1QyXpfUbsxbVDJel9RuzFlquMt0gSp7OkHbsLIlqXczSyP5ZkXbX31MiLUd5VeFq&ccb=13-1&oh=06_Q399iq2-VlX30yq_-TCjQJ9BrwVogE3xdFvflhbjRS5_Fhw&oe=661ED752&_nc_sid=ef6713",
                                    "width": 640
                                }
                            },
                            "target": {
                                "url": "https://l.facebook.com/l.php?u=https%3A%2F%2Fgist.github.com%2Fhuoshan12345%2F44b1b4927b21d4ec21d1cbd61ea659da&h=AT3dxbg1xtQWjJC9x6KwgcKNBsSoFsDvxUFG1SxOF-wqtkq-NaFtjbyvVXt9cppceIGk-PjzRZRiuJRkKZT0qpWERnJhB80PJxUy2zhw877aIVVw0fbBD_ag2Ie0J1i4CAOMksznwAA&s=1"
                            },
                            "title": "Instagram enc_password generator in C#",
                            "type": "share",
                            "url": "https://l.facebook.com/l.php?u=https%3A%2F%2Fgist.github.com%2Fhuoshan12345%2F44b1b4927b21d4ec21d1cbd61ea659da&h=AT3dxbg1xtQWjJC9x6KwgcKNBsSoFsDvxUFG1SxOF-wqtkq-NaFtjbyvVXt9cppceIGk-PjzRZRiuJRkKZT0qpWERnJhB80PJxUy2zhw877aIVVw0fbBD_ag2Ie0J1i4CAOMksznwAA&s=1"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 10
                    }
                },
                "shares": {
                    "count": 2
                }
            },
            {
                "id": "1777766135578951_7527932260562281",
                "created_time": "2024-04-13T23:12:06+07:00",
                "message": "Cần học train yolo bằng python ae nào dạy ib em với \nTele: @hunght1890\nCó sẵn file data",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 7
                    }
                }
            },
            {
                "id": "1777766135578951_7529987630356744",
                "created_time": "2024-04-14T11:43:03+07:00",
                "message": "Xin đừng lạnh lùng lướt qua ! 1 Chia sẻ công đức vô lượng\n#GÓC KÊU GỌi Áo Quan cho 2 cháu bị đuối nước \n1/ cháu Trần Minh Đức ( 8 tuổi )\n2/ cháu Trần Minh Tuấn ( 6 tuổi ) \nNgười mẹ bất lực khóc kêu thảm thiết khi nghe con đuối nước mà không tìm đc xác Đây là hoàn cảnh quá đáng thương của Chị LỘC 45 tuổi  Quê ở Lệ Thủy Quảng Bình\nBản thân gia đình chị có chồng ốm yếu, đau ốm triền miên, cuộc sống vô cùng vất vả, sinh được 2 đứa con trai là niềm vui là chỗ dựa cũng là niềm hạnh phúc để chị vượt qua khốn khó. Nhưng cuộc đời ko mỉm cười với chị. 2 em không may mắn do đi bắt ốc phụ gia đình đã bị đuối nước 2 ngày sau mới tìm đc xác \nGia đình khó khăn chị mong muốn có chiếc quan tài để mai táng cho 2 cháu ra đi yên nghỉ\nGiờ đây chị vô cùng hụt hẫn nằm bên xác 2 con không còn nữa, Không còn vui đùa như trước nữa. Bao nhiêu tuổi hờn giờ đây đối với chị coi như đã tắt. Cái chết và sống bây giờ là một. C ko ăn, ko uống mấy ngày ni, ko dậy nổi, chỉ nằm ôm 2 đứa để sưởi ấm giữa ngôi nhà đang ngập nước. Mong mọi người giúp đỡ gd chị ấy một miếng khi đói bằng gói khi no.( không tiền lo cho 2 con chi phí mai táng ) nhìn mà tội các bé  \n🙏 Nay mọi người đứng ra kêu gọi hộ gia đình mong Quý Mạnh Thường Quân gieo duyên giúp đỡ chị LỘC và Anh Thịnh có chi phí mai táng cho 2 bé để 2 bé có thể an nghỉ qua STK của Chị LỘC mẹ 2 cháu ;\n- STK : 551123280\n- CTK : LÊ THỊ LỘC\n- Ngân hàng : MB BANK\n✅Nội dung: U/H chị LỘC chi phi mai táng 2 cháu\n✅Mọi sự ủng hộ được cập nhật trực tiếp tại cmt của bài kêu gọi.\n------------------------------------------------------------------\n11:42:51\n- Em xin 1 chia sẻ để nhiều người biết về hoàn cảnh đáng thương của chị ạ\n- Chi ân công đức của mọi người vô lượng\n- Chúc quý ân nhân MTQ hạnh phúc an lạc !!!",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 960,
                                    "src": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-6/435871057_347414191656578_1151113905554246795_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeH-CEgpLPrmrRYYr7991xcVTuqYAGxqWLpO6pgAbGpYuoQ2C21d3J8hMAoS95Sl1iUkzB3aK_7pmSNroCBmdmLS&_nc_ohc=RXffXrevRh8Ab5sqfic&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfA2JLRRx1M1NeSrqg4dNqZF4tk6CK9uqrU4gySAxk3DVA&oe=6622D02C",
                                    "width": 720
                                }
                            },
                            "target": {
                                "id": "7529987630356744",
                                "url": "https://www.facebook.com/media/set/?set=pcb.7529987630356744&type=1"
                            },
                            "title": "Ảnh từ bài viết của Luat Bui",
                            "type": "album",
                            "url": "https://www.facebook.com/media/set/?set=pcb.7529987630356744&type=1",
                            "subattachments": {
                                "data": [
                                    {
                                        "media": {
                                            "image": {
                                                "height": 960,
                                                "src": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-6/435871057_347414191656578_1151113905554246795_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeH-CEgpLPrmrRYYr7991xcVTuqYAGxqWLpO6pgAbGpYuoQ2C21d3J8hMAoS95Sl1iUkzB3aK_7pmSNroCBmdmLS&_nc_ohc=RXffXrevRh8Ab5sqfic&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfA2JLRRx1M1NeSrqg4dNqZF4tk6CK9uqrU4gySAxk3DVA&oe=6622D02C",
                                                "width": 720
                                            }
                                        },
                                        "target": {
                                            "id": "347414201656577",
                                            "url": "https://www.facebook.com/photo.php?fbid=347414201656577&set=gm.7529987633690077&type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/photo.php?fbid=347414201656577&set=gm.7529987633690077&type=3"
                                    },
                                    {
                                        "media": {
                                            "image": {
                                                "height": 960,
                                                "src": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t39.30808-6/435569182_347414188323245_2637734008615890102_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeF42Ix9Ji2ELyaIe9NHcZ5hg2VadG75sNqDZVp0bvmw2rEulm_UUGlA_M59RyR_0a4tsBrHuQK3l0i3KzBlmUtZ&_nc_ohc=NXhvM5gkMrcAb5Ahq-2&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfA2l_sH4F36RQcFGl1Qgjbt4NlFJRxNy1aRttbucCjC_g&oe=6622C1AE",
                                                "width": 537
                                            }
                                        },
                                        "target": {
                                            "id": "347414208323243",
                                            "url": "https://www.facebook.com/photo.php?fbid=347414208323243&set=gm.7529987637023410&type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/photo.php?fbid=347414208323243&set=gm.7529987637023410&type=3"
                                    },
                                    {
                                        "media": {
                                            "image": {
                                                "height": 960,
                                                "src": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-6/435894614_347414194989911_5730437638280034152_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEwlle8JCL6O5PmvhOJ8PAMz3eDsqnub3vPd4Oyqe5ve3ENv0fynHVeyg8HfqKtWKW9DN-f1h-w4Qrr1QTdvkcU&_nc_ohc=HTG8yxWmgoMAb5yhZsW&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfBLr5iwa9jewiaiVH3Y1kjmKhiGkecX-L2QQPJU5934iw&oe=6622D4D2",
                                                "width": 538
                                            }
                                        },
                                        "target": {
                                            "id": "347414204989910",
                                            "url": "https://www.facebook.com/photo.php?fbid=347414204989910&set=gm.7529987627023411&type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/photo.php?fbid=347414204989910&set=gm.7529987627023411&type=3"
                                    }
                                ]
                            }
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                }
            },
            {
                "id": "1777766135578951_7525885320766975",
                "created_time": "2024-04-13T11:58:42+07:00",
                "message": "Các bác cho e hỏi chút, e dùng js để send các kí tự đặc biệt vào textbox nhưng sau khi set value cho nó thì textbox k hiển thị chuỗi string có chứa các kí tự đặc biệt BMP đó thì làm sao để set được value nhỉ (có thể textbox đó chặn set giá trị bằng js)? Cho em xin giải pháp !",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 2
                    }
                }
            },
            {
                "id": "1777766135578951_7529719770383530",
                "created_time": "2024-04-14T10:03:29+07:00",
                "message": "Chuyên mục giải captcha trên giả lập, hcaptcha,fun,… Cần hỗ trợ ạ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7523669460988561",
                "created_time": "2024-04-12T23:48:09+07:00",
                "message": "Cần tìm 1 bác reverse engineering APK,\nbác nào làm được CMT e ib ạ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 2
                    }
                }
            },
            {
                "id": "1777766135578951_7527839070571600",
                "created_time": "2024-04-13T22:46:51+07:00",
                "message": "Trong nhóm mình có ai đào tạo Pc control C# k ạ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7526171474071693",
                "created_time": "2024-04-13T13:40:07+07:00",
                "message": "Có bác nào có source code auto mở LDPlayer tùy theo số lượng rồi add vào panel không ạ em xin tham khảo code với ạ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                }
            },
            {
                "id": "1777766135578951_6747257921963056",
                "created_time": "2023-09-22T21:53:45+07:00",
                "message": "Khách đặt làm tool Telegram xong rồi bom tiền cọc nên em bán lẻ gỡ gạc lại ít tiền 😅\n\nTool dành cho các bác lập nhóm bắn tín hiệu, chơi Crypto, forex, chứng khoán, ...\n\nTÍNH NĂNG\n- Nằm vùng, tự động copy khi có bài đăng mới trong Channel/Group đối thủ.\n- Hoạt động với cả Channel/Group để chế độ private.\n- Hoạt động với cả Channel/Group bật chế độ chống sao chép bài viết.\n- Tự động thêm chữ ký vào bài viết.\n\nBán lẻ 500k, hạn sử dụng vĩnh viễn, bảo hành trọn đời. Có thể chạy nhiều acc trên nhiều máy tính cùng lúc.",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 720,
                                    "src": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.30808-6/381978096_1760671044370725_2012117047701664313_n.jpg?stp=dst-jpg_p720x720&_nc_cat=109&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEPbuShVm2zbJbDLE2ItO26rVDZmGj75S-tUNmYaPvlL_QE62OHVzb0RD6epKy5F813eXTnYo4f9sCl3DDi8_BB&_nc_ohc=cmAIXabDrJcAb7lSfBK&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfCLVcEGNN94U3YaJHaOOUlmt4DcWzI2urkAqXZAVP67dw&oe=6622C1AD",
                                    "width": 1510
                                }
                            },
                            "target": {
                                "id": "1760671057704057",
                                "url": "https://www.facebook.com/photo.php?fbid=1760671057704057&set=gm.6747257921963056&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=1760671057704057&set=gm.6747257921963056&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 9
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 39
                    }
                }
            },
            {
                "id": "1777766135578951_7522002914488549",
                "created_time": "2024-04-12T15:14:42+07:00",
                "message": "Cần mua code giải geetest captcha sử dụng selenium c# b nào có để lại cmt mình inbox",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 2
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 2
                    }
                }
            },
            {
                "id": "1777766135578951_5487890481233146",
                "created_time": "2022-08-22T15:54:33+07:00",
                "message": "#hoidap Mình làm tới đây. Bác nào có thể chỉ cho mình làm sao dùng adb thay đổi proxy từ GridView qua ldplayer không hay phải dùng click và sent text từng cái sang ldplayer quản lý wifi - proxy?",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 720,
                                    "src": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.30808-6/300344615_3419874908332881_814028324362783819_n.jpg?stp=dst-jpg_p720x720&_nc_cat=102&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEQ4j0nBUlX4AVjDrvwDXowDQHXTMEP3IINAddMwQ_cghoicD0w4eXM4BHlk6p1qr0vGkPA8V9MWMzosbh8S5T6&_nc_ohc=bccU0dGyhPQAb6gCrx-&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfDnXEKW02NF5i3MRDG8hUaoAyb1la69v9fxnnTvjPWYZQ&oe=6622AAE6",
                                    "width": 1268
                                }
                            },
                            "target": {
                                "id": "3419874911666214",
                                "url": "https://www.facebook.com/photo.php?fbid=3419874911666214&set=gm.5487890481233146&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=3419874911666214&set=gm.5487890481233146&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 14
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 32
                    }
                },
                "shares": {
                    "count": 1
                }
            },
            {
                "id": "1777766135578951_5529818960373631",
                "created_time": "2022-09-06T19:21:04+07:00",
                "message": "Mọi người trong group có ai biết cách đẩy View của LDPlayer vào trong GUI như hình bên dưới đây không ạ? Cho e xin keyword e cảm ơn.",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 236,
                                    "src": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.30808-6/302736194_2044919999026905_9091821414841502755_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeH1Vk4eulpybnsKzNRFlr4j3YXpvP7vKuPdhem8_u8q44vJOdf7CmVpqtP6Pp1U-4cmOl7M4-ckho-FpMxQ9sma&_nc_ohc=OPZbb96pK4oAb6mki1d&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfD96_dcTjdsfyc6pqNxPTissG1ggnmyWow8_kW7RyeXxA&oe=6622C8B5",
                                    "width": 464
                                }
                            },
                            "target": {
                                "id": "2044920002360238",
                                "url": "https://www.facebook.com/photo.php?fbid=2044920002360238&set=gm.5529818960373631&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=2044920002360238&set=gm.5529818960373631&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 4
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 9
                    }
                }
            },
            {
                "id": "1777766135578951_7525696827452491",
                "created_time": "2024-04-13T10:50:50+07:00",
                "message": "E khởi động chrome với selenium python. Mà cứ mỗi lần tạo profile mới nó lại nhảy ra cái này. Các bác biết agr nào chặn tự động mở cái này không ạ",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 463,
                                    "src": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.30808-6/437858562_3778793939031868_7921224634508196599_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEfyI6nOlYP5jbNoqyvCa_-RxIlh-W-k-NHEiWH5b6T44irGz83BR7lPcnCosZzmUvW-V2og4__2vbxosjqkps4&_nc_ohc=XMC9ggNVt3UAb5W4CJz&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfA2W0P99_EaTXC5eWlpoyn1ExKk59PkndKi6pJUmMGNXA&oe=6622A338",
                                    "width": 598
                                }
                            },
                            "target": {
                                "id": "7525696827452491",
                                "url": "https://www.facebook.com/media/set/?set=pcb.7525696827452491&type=1"
                            },
                            "title": "Ảnh từ bài viết của Nguyễn Mai",
                            "type": "album",
                            "url": "https://www.facebook.com/media/set/?set=pcb.7525696827452491&type=1",
                            "subattachments": {
                                "data": [
                                    {
                                        "media": {
                                            "image": {
                                                "height": 463,
                                                "src": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.30808-6/437858562_3778793939031868_7921224634508196599_n.jpg?_nc_cat=111&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEfyI6nOlYP5jbNoqyvCa_-RxIlh-W-k-NHEiWH5b6T44irGz83BR7lPcnCosZzmUvW-V2og4__2vbxosjqkps4&_nc_ohc=XMC9ggNVt3UAb5W4CJz&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfA2W0P99_EaTXC5eWlpoyn1ExKk59PkndKi6pJUmMGNXA&oe=6622A338",
                                                "width": 598
                                            }
                                        },
                                        "target": {
                                            "id": "3778793949031867",
                                            "url": "https://www.facebook.com/photo.php?fbid=3778793949031867&set=gm.7525696824119158&type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/photo.php?fbid=3778793949031867&set=gm.7525696824119158&type=3"
                                    },
                                    {
                                        "media": {
                                            "image": {
                                                "height": 392,
                                                "src": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.30808-6/437914772_3778793929031869_278761550749157498_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHGkb1OAHMJg1Z6UPWSbC2hgf6vqVwOe_uB_q-pXA57-2Rppn3V8j8-W7ZA_IN9dukD8D-uhXU5V--4odLnFNEr&_nc_ohc=OBq1ywa65isAb7zxwtB&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfD0HJq7XaXj0lkDHKUWbBsgcO0SkM6uVCYFIrlQRSPT7Q&oe=6622AFB4",
                                                "width": 354
                                            }
                                        },
                                        "target": {
                                            "id": "3778793942365201",
                                            "url": "https://www.facebook.com/photo.php?fbid=3778793942365201&set=gm.7525696830785824&type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/photo.php?fbid=3778793942365201&set=gm.7525696830785824&type=3"
                                    }
                                ]
                            }
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                }
            },
            {
                "id": "1777766135578951_7518866364802204",
                "created_time": "2024-04-11T21:32:20+07:00",
                "message": "Em cần mua schema url vào thẳng tab post reels trên app Facebook android ạ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 2
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7521106527911521",
                "created_time": "2024-04-12T09:58:18+07:00",
                "message": "Vẫn cần người làm tool game theo yêu cầu. Ai thực sự nhận ib.",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 4
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 4
                    }
                }
            },
            {
                "id": "1777766135578951_7519451088077065",
                "created_time": "2024-04-12T00:28:31+07:00",
                "message": "Ae cẩn thận thanh niên này nhé ultra mở cmd và paste code nếu mình nhìn ko nhầm thì get cookie trỏ về web nó",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 1200,
                                    "src": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.30808-6/435098140_949162777001018_4728876093126895645_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeFL5Av68DmDKhl6TJk_SWFZnybRQtfiTYGfJtFC1-JNgb06n4N6B-dHvMEVteOuVrWlb4KqQkoBjvyDw5nFDpK2&_nc_ohc=tWGRWkVC71cAb4V-9yW&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfBtPvvkL7eA39zYI2bzwo5JPcjQOWrSE505kpawTQ7b7Q&oe=6622B3F4",
                                    "width": 540
                                }
                            },
                            "target": {
                                "id": "949162783667684",
                                "url": "https://www.facebook.com/3736994476575517/photos/gm.7519451088077065/949162783667684/?type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/3736994476575517/photos/gm.7519451088077065/949162783667684/?type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 7
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 16
                    }
                }
            },
            {
                "id": "1777766135578951_7522062954482545",
                "created_time": "2024-04-12T15:35:52+07:00",
                "message": "Cần bạn nào viết c# game nro lậu, đa chức năng mod code , bạn nào nhận ib mình",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                }
            },
            {
                "id": "1777766135578951_7523234427698731",
                "created_time": "2024-04-12T21:44:02+07:00",
                "message": "Có ai biết khóa học về c# nào ko ạ chỉ cho e với e mới tìm tòi để học làm game\ncảm ơn ạ!!!",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7521222901233217",
                "created_time": "2024-04-12T10:41:43+07:00",
                "message": "cần mua 1k nick gmail bị xác minh add thêm sdt mới, bác nào bỏ đi bán lại e vs =))",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 2
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_3781258695229675",
                "created_time": "2021-01-31T13:38:14+07:00",
                "message": "demo code sử dụng adb và opencv điều khiển ldplayer cho người mới.\nSetup ldplayer độ phân giải 720*1280, adb chế độ gỡ lỗi cục bộ hoặc từ xa.\nCopy thư mục Data vào khu vực Debug để nhận diện ảnh.\nhttps://secufiles.com/72hp/SearchImg.rar",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 405,
                                    "src": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t15.5256-10/140160783_450051633044378_5098069485716592148_n.jpg?stp=dst-jpg_s720x720&_nc_cat=100&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEHVx3l2KAJAX3WTbb8w94uR1U6ZI-BvIxHVTpkj4G8jL5Dz3J8E6zs80hsaF90d5mHXDmBKyqTtXF1ZMBRi6LC&_nc_ohc=HPxcppuUKZUAb68IWja&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfB2FivfyEBDqmc0-16GRRPnVSg4Nj9TVv2Oe16uDyTSuQ&oe=6622CD79",
                                    "width": 720
                                },
                                "source": "https://scontent.fsgn2-11.fna.fbcdn.net/o1/v/t2/f1/m69/GGqbHBnZD-xUXAEBAJms6KbgdDkVbmdjAAAF.mp4?efg=eyJ2ZW5jb2RlX3RhZyI6Im9lcF9oZCJ9&_nc_ht=scontent.fsgn2-11.fna.fbcdn.net&_nc_cat=103&_nc_eui2=AeGQL8xvfPLHnOunXI_nxhBqdxeLQrKwuh53F4tCsrC6HmUbsV0ZmvZZPlinzZJyv3w3IY7a9zG97iPGMzFisfrD&strext=1&vs=e28aaf45fc9f854a&_nc_vs=HBksFQIYOnBhc3N0aHJvdWdoX2V2ZXJzdG9yZS9HR3FiSEJuWkQteFVYQUVCQUptczZLYmdkRGtWYm1kakFBQUYVAALIAQAVAhg6cGFzc3Rocm91Z2hfZXZlcnN0b3JlL0dCdGZuUWkwNnRkMVN1MEpBQkpBejN5RjlHVUxidjRHQUFBRhUCAsgBAEsHiBJwcm9ncmVzc2l2ZV9yZWNpcGUBMQ1zdWJzYW1wbGVfZnBzABB2bWFmX2VuYWJsZV9uc3ViACBtZWFzdXJlX29yaWdpbmFsX3Jlc29sdXRpb25fc3NpbQAoY29tcHV0ZV9zc2ltX29ubHlfYXRfb3JpZ2luYWxfcmVzb2x1dGlvbgAddXNlX2xhbmN6b3NfZm9yX3ZxbV91cHNjYWxpbmcAEWRpc2FibGVfcG9zdF9wdnFzABUAJQAcjBdAAAAAAAAAABERAAAAJui5gcmj8dUKFQIoAkMzGAt2dHNfcHJldmlldxwXQGr3dLxqfvoYIWRhc2hfZ2VuMmh3YmFzaWNfaHEyX2ZyYWdfMl92aWRlbxIAGBh2aWRlb3MudnRzLmNhbGxiYWNrLnByb2Q4ElZJREVPX1ZJRVdfUkVRVUVTVBsKiBVvZW1fdGFyZ2V0X2VuY29kZV90YWcGb2VwX2hkE29lbV9yZXF1ZXN0X3RpbWVfbXMBMAxvZW1fY2ZnX3J1bGUHdW5tdXRlZBNvZW1fcm9pX3JlYWNoX2NvdW50BTI5OTA5EW9lbV9pc19leHBlcmltZW50AAxvZW1fdmlkZW9faWQPNDUwMDQ5NjQ5NzExMjQzEm9lbV92aWRlb19hc3NldF9pZBAzMDAzNjEyODQ2NTU4MDI1FW9lbV92aWRlb19yZXNvdXJjZV9pZBAzMDAzNjEyODQzMjI0NjkyHG9lbV9zb3VyY2VfdmlkZW9fZW5jb2RpbmdfaWQQMTQ1MTM0ODUzMjQ1ODM2NA52dHNfcmVxdWVzdF9pZAAlAhwAJcQBGweIAXMDMzk3AmNkCjIwMjEtMDEtMzADcmNiBTI5OTAwA2FwcA5GYWNlYm9vayBUb3VjaAJjdApHUk9VUF9QT1NUE29yaWdpbmFsX2R1cmF0aW9uX3MKMjE1Ljc4NjY0NgJ0cxVwcm9ncmVzc2l2ZV9lbmNvZGluZ3MA&ccb=9-4&oh=00_AfAWAACVtQBcFvdJt45HKgQY4pQgiPbdktM8Ay503nSVRw&oe=661EC00A&_nc_sid=1d576d&_nc_rid=568647487771561&_nc_store_type=1"
                            },
                            "target": {
                                "id": "450049649711243",
                                "url": "https://www.facebook.com/groups/autocsharp/permalink/3781258695229675/"
                            },
                            "type": "video_autoplay",
                            "url": "https://www.facebook.com/groups/autocsharp/permalink/3781258695229675/"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 8
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 62
                    }
                },
                "shares": {
                    "count": 12
                }
            },
            {
                "id": "1777766135578951_7523048934383947",
                "created_time": "2024-04-12T20:50:25+07:00",
                "message": "mình đang cần 1 bạn biết lập trình code c# có 1 con game đang cần sửa ai làm được ib scam thì né cho đỡ mất thời gian",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 6
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 5
                    }
                }
            },
            {
                "id": "1777766135578951_7517393471616160",
                "created_time": "2024-04-11T14:03:51+07:00",
                "message": "Em tìm người viết app android sẽ tự động fake proxy qua lệnh adb được gọi ạ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 15
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 13
                    }
                }
            },
            {
                "id": "1777766135578951_7476790699009771",
                "created_time": "2024-04-02T00:25:44+07:00",
                "message": "Thấy nhiều bạn có nhu cầu tạo khóa học Selenium C#. Nên mình dự định sẽ mở 1 khóa cấp tốc online. Mọi người có nhu cầu để lại bình luận để mình xem đủ 10 người mở lớp nha.\n\nBạn nào muốn học mà chưa được add vào nhóm fb thì ib mình nha",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 55
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 86
                    }
                }
            },
            {
                "id": "1777766135578951_7519080374780803",
                "created_time": "2024-04-11T22:35:34+07:00",
                "message": "Cần một bác viết scritp chạy được trên nền tảng change phone của https://bipdevice.io/\nTool này có mục auto để chạy các script viết thêm vào",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                }
            },
            {
                "id": "1777766135578951_7514559471899560",
                "created_time": "2024-04-10T21:57:53+07:00",
                "message": "có ai chạy auto click bài khảo sát giá rẻ kh ạ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7211148875573956",
                "created_time": "2024-01-26T11:49:40+07:00",
                "message": "cần source tạo profile gologin không thông qua gologin, để giá dưới comment e tự ib nhé",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 6
                    }
                },
                "shares": {
                    "count": 1
                }
            },
            {
                "id": "1777766135578951_7461686303853544",
                "created_time": "2024-03-29T12:28:47+07:00",
                "message": "dịch vụ giải captcha bên twitter sử dụng bên nào ổn vậy mấy anh, có tích hợp api key bằng c# đc ko",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 429,
                                    "src": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.30808-6/434645227_425641416619262_4198275379674164928_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeGgTkfe5aiz2PXbiztozSzkLb5RjeAJEqEtvlGN4AkSoacntvRVuE8EUgnGXWX-7hUMSnqfsMXCRzWWB2mgeMcp&_nc_ohc=LouCrt_t8y8Ab50JNFx&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfDGZPRUg8Po1gh4ctdW-ukLLXDaF3pcRmLYtwbUvIA3qg&oe=6622B468",
                                    "width": 447
                                }
                            },
                            "target": {
                                "id": "425641419952595",
                                "url": "https://www.facebook.com/photo.php?fbid=425641419952595&set=gm.7461686303853544&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=425641419952595&set=gm.7461686303853544&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 5
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                }
            },
            {
                "id": "1777766135578951_6352146404807545",
                "created_time": "2023-05-31T00:59:08+07:00",
                "message": "Hiii. Hôm nay e xin phép share ae 1 tool kết nối proxy nho nhỏ ạ cho team e phát triển ạ.\n\n*Ưu điểm:\n   + Hỗ trợ HTTP và Shock5\n   + Hỗ trợ proxy authentication (có user - pass)\n   + Hỗ trợ đổi IP qua CMD (không cần phải click trên UI)\n   + Có chức năng tự động đổi IP theo thời gian hẹn trước bằng api của Tinsoft, Shoplike.\n   + Change ip khá sâu.\n* Nhược điểm:\n   + Đổi ip khá chậm (khoảng 5-10s sau mới nhận IP mới)\n   + Là bản beta nên có nhiều lỗi phát sinh.\n\nCMD:\n   - Đổi IP: adb shell am broadcast -a com.vat.vpn.CONNECT_PROXY -n com.vat.vpn/.ui.ProxyReceiver --es address \\\"\\\" --es port \\\"\\\" --es username \\\"\\\" --es password \\\"\\\"\n   - Tự động đổi IP: adb shell am broadcast -a com.vat.vpn.AUTO_CONNECT_PROXY -n com.vat.vpn/.ui.ProxyReceiver --es website \\\"\\\" --es api_key \\\"\\\" --ei timer 2 --ez auto_change true\"\n\nLink: ",
                "attachments": {
                    "data": [
                        {
                            "target": {
                                "url": "https://l.facebook.com/l.php?u=https%3A%2F%2Fdrive.google.com%2Ffile%2Fd%2F1PYoYID6qM35zkn5Ph1nk3kNo3iKJS59x%2Fview%3Fusp%3Dshare_link&h=AT0puRwWEXXL21uzz2KYJ7MPSD7ROV6Yr3Z5xYK1IP-o-8W78GP26KBxYtxe3pRrp3_i-CsW6owr3V6QzXk7aoSRjh_IWJ0uXNqod-k374biN0dpS2qUmCYQnBTDisKxX4ezKH953Rk&s=1"
                            },
                            "title": "VAT-VpnProxy_v1.0.0.apk",
                            "type": "share",
                            "url": "https://l.facebook.com/l.php?u=https%3A%2F%2Fdrive.google.com%2Ffile%2Fd%2F1PYoYID6qM35zkn5Ph1nk3kNo3iKJS59x%2Fview%3Fusp%3Dshare_link&h=AT0puRwWEXXL21uzz2KYJ7MPSD7ROV6Yr3Z5xYK1IP-o-8W78GP26KBxYtxe3pRrp3_i-CsW6owr3V6QzXk7aoSRjh_IWJ0uXNqod-k374biN0dpS2qUmCYQnBTDisKxX4ezKH953Rk&s=1"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 20
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 109
                    }
                },
                "shares": {
                    "count": 21
                }
            },
            {
                "id": "1777766135578951_7317848254904017",
                "created_time": "2024-02-22T08:45:18+07:00",
                "message": "Em dùng auto chrome để like , follow twitter được vài lần thì bị logout khỏi . Các bác cho em hỏi lý do do đâu ạ.",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 720,
                                    "src": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.30808-6/428679087_1435470057045568_1835870208018489157_n.jpg?stp=dst-jpg_p720x720&_nc_cat=111&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeF_YWAk9qRVuvYsnnzT34f6aritxH65gQ5quK3EfrmBDmy1TiZoka4GgwORXyj50AGdPxDSLqPLo2aymVK2BHEy&_nc_ohc=TaKqe3zkFaoAb5wv6Ks&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfARhKSpiZ8ul4o9o7tNp_Ttp7XxXNg7YZWMW-ntGudf9g&oe=6622A171",
                                    "width": 1377
                                }
                            },
                            "target": {
                                "id": "1435470060378901",
                                "url": "https://www.facebook.com/photo.php?fbid=1435470060378901&set=gm.7317848254904017&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=1435470060378901&set=gm.7317848254904017&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 11
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 18
                    }
                }
            },
            {
                "id": "1777766135578951_7497794410242733",
                "created_time": "2024-04-06T21:17:16+07:00",
                "message": "Cho e hỏi tool reg twitter của em mấy hôm nay bị như này , Có ai cũng bị tương tự không ạ, twitter mới update gì hả các bác ?",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 720,
                                    "src": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.30808-6/423716658_1084313902845802_8707649604087227558_n.png?stp=dst-png_p720x720&_nc_cat=100&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeG0Wvl4bZpvjNNV_nXKH6_R1aGrVxYk4b_VoatXFiThv1evO_qLaAT4md-Y5vwSRLZoC-4vCTdtxIZuHB2TZeTe&_nc_ohc=Lm7D-MTL-HoAb6_QGv3&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfD593wYB1AeWr3H1rLIR_W0SE3o-xrfRKYApNGJuowXsw&oe=66229E63",
                                    "width": 757
                                }
                            },
                            "target": {
                                "id": "1084313909512468",
                                "url": "https://www.facebook.com/1031957964748063/photos/gm.7497794410242733/1084313909512468/?type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/1031957964748063/photos/gm.7497794410242733/1084313909512468/?type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                }
            },
            {
                "id": "1777766135578951_7480776758611165",
                "created_time": "2024-04-02T22:45:09+07:00",
                "message": "Mùa này xài twitter hao acc quá nên mình có phải code tool unlock acc twitter. Lang thang thì kiếm đc tool mấy anh nga ngố nên đem về sửa lại mắm muối thấy chạy khá ngon nên chia sẻ cho anh em test thử.\nAe chạy thử thì cho mình xin ít kinh nghiệm tránh block ạ. Chủ yếu mình cần view tweet, re tweet mà còn gà vẫn chưa nắm được ngưỡng.\nQuay trở lại cái tool thì\n- Mấy anh này code bất đồng bộ của python + check status và unlock bằng http request nên máy yếu anh em vẫn có thể chạy được rất nhiều thread (chỉnh bằng cấu hình MAX_THREADS) và tốn ít CPU, hơn hẳn ae xài đa luồng và điều khiển chrome (như trước mình đã thử unlock bằng sele).\n- Chạy xong tool tự phân loại tài khoản về thư mục input-output\n- Mình có sửa lại code dùng api Rockcaptcha (cũng dùng bất đồng bộ luôn), bên này giải 1$ được 1k token. Tốc độ giải trung bình 1s nên mình check vài ngàn acc để unlock mà chỉ mất khoảng một vài phút.\nTiện thể ae có cần đăng ký rockcaptcha thì dùng link ref để ủng hộ mình viết thêm vài bài chia sẻ nữa nha.\nLink đăng ký rock: https://rockcaptcha.com?affref=36411\nTool và hướng dẫn chạy thì mình sẽ để dưới comment. Ae có thắc nào cứ comment nhé mình sẽ cố gắng hỗ trợ.",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 720,
                                    "src": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.30808-6/434667389_737259161929547_7221806480302040604_n.jpg?stp=dst-jpg_p720x720&_nc_cat=111&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEAX4P_QAQgsqXLXBFLDVKOZo9iBRm_6zZmj2IFGb_rNlERBkBfaMNgs1xcLw-xNjquDO7DW5tAvcf3I2KZEanJ&_nc_ohc=nM4tF-O520IAb5jW9sC&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfCXPKjLUI7o2dNt-0ehOsCCZdiPIn_56Y-rZ_eHMl3Ikg&oe=6622D4BC",
                                    "width": 879
                                }
                            },
                            "target": {
                                "id": "7480776758611165",
                                "url": "https://www.facebook.com/media/set/?set=pcb.7480776758611165&type=1"
                            },
                            "title": "Ảnh từ bài viết của Quang Minh",
                            "type": "album",
                            "url": "https://www.facebook.com/media/set/?set=pcb.7480776758611165&type=1",
                            "subattachments": {
                                "data": [
                                    {
                                        "media": {
                                            "image": {
                                                "height": 720,
                                                "src": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.30808-6/434667389_737259161929547_7221806480302040604_n.jpg?stp=dst-jpg_p720x720&_nc_cat=111&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEAX4P_QAQgsqXLXBFLDVKOZo9iBRm_6zZmj2IFGb_rNlERBkBfaMNgs1xcLw-xNjquDO7DW5tAvcf3I2KZEanJ&_nc_ohc=nM4tF-O520IAb5jW9sC&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfCXPKjLUI7o2dNt-0ehOsCCZdiPIn_56Y-rZ_eHMl3Ikg&oe=6622D4BC",
                                                "width": 879
                                            }
                                        },
                                        "target": {
                                            "id": "737259165262880",
                                            "url": "https://www.facebook.com/photo.php?fbid=737259165262880&set=gm.7480776751944499&type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/photo.php?fbid=737259165262880&set=gm.7480776751944499&type=3"
                                    },
                                    {
                                        "media": {
                                            "image": {
                                                "height": 716,
                                                "src": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.30808-6/434687975_737259208596209_1179750985776433186_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeFnEdozRy3WtWEEaJV4PjBKruqXz7Qx-Lau6pfPtDH4ts9rIFpFD6ZhkRm0V3K3T-gRIEuqU12Y2mpmPCayYm3H&_nc_ohc=eH8sI3VTXmAAb4S7NuD&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfC0dl7RXyTo1Gcdk7RPsqoi3OWqA9CYdRmuURuA9AOUdQ&oe=6622B990",
                                                "width": 1280
                                            }
                                        },
                                        "target": {
                                            "id": "737259215262875",
                                            "url": "https://www.facebook.com/photo.php?fbid=737259215262875&set=gm.7480776755277832&type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/photo.php?fbid=737259215262875&set=gm.7480776755277832&type=3"
                                    }
                                ]
                            }
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 23
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 77
                    }
                },
                "shares": {
                    "count": 12
                }
            },
            {
                "id": "1777766135578951_7514873108534863",
                "created_time": "2024-04-10T23:36:25+07:00",
                "message": "Bác nào biết quy trình reg tiktok browser mà k bị nhả tương tác k ạ :(",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 2
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 2
                    }
                }
            },
            {
                "id": "1777766135578951_7517009614987879",
                "created_time": "2024-04-11T12:03:25+07:00",
                "message": "Thấy nhiều bác inbox hỏi đoạn Add LD vào Form WPF. E up lại file lúc trước có bác chia sẽ trong nhóm. Mở ra đọc code vui lòng không inbox hỏi thêm.\nhttps://drive.google[.]com/file/d/1v4Oj2ks5R7Y5th5vk9P4S3oiial0-uce/view?usp=sharing",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 8
                    }
                },
                "shares": {
                    "count": 3
                }
            },
            {
                "id": "1777766135578951_7516784465010394",
                "created_time": "2024-04-11T10:49:57+07:00",
                "message": "để tạo được kiểu tab menu ntn trong winform devexpress dùng gì vậy mn , kiểu như tab google chorme\nthank all mn",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 41,
                                    "src": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.30808-6/436187340_332413789454110_2055567729043319257_n.png?_nc_cat=102&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeGxKDxaJUk5-2r3dujANjGHwk3P_70MN4DCTc__vQw3gMrEugIlCmr3_MmkIV4J5YbF2OihgenIit_FL0kCSmgL&_nc_ohc=vF87xAPJ4BkAb60nPEL&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfBE7WjtVa3xWyiQHPUVzIWI5kQMjv-Y8gGuNwK7b9pDaQ&oe=6622B51E",
                                    "width": 523
                                }
                            },
                            "target": {
                                "id": "332413792787443",
                                "url": "https://www.facebook.com/332413162787506/photos/gm.7516784465010394/332413792787443/?type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/332413162787506/photos/gm.7516784465010394/332413792787443/?type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                }
            },
            {
                "id": "1777766135578951_7508973532458154",
                "created_time": "2024-04-09T13:46:52+07:00",
                "message": "Tự dưng gần đây một loạt gmail clone của mình bị thế này, login mở tay ko được. Xin hỏi các thầy nó còn cứu được không? Mình thường xuyên mở chrome bằng autoit với bộ tham số trong ảnh. Các thầy cho em xin ít bật mí em tìm chén thánh với, chứ gmail die nhiều làm em đang khủng hoảng tài nguyên quá. Nếu ko share được thì bán em mua cũng được ạ!",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 636,
                                    "src": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-6/434996395_1368587073828864_1287516045038210399_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeG8g10UvPspuPTXUBcRyQDE8N3ClUTbLfTw3cKVRNst9FFQk0qW9-VMY-ITZ1-d6K3KmS0-spm5p_qtd2O0Vq2F&_nc_ohc=-zxUgXL3KhwAb6OlB10&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfCxwdqLBwSJpzmjcde_fDAMfdKv3Z9aPVcOtYJgrp0cnA&oe=6622B9C6",
                                    "width": 542
                                }
                            },
                            "target": {
                                "id": "7508973532458154",
                                "url": "https://www.facebook.com/media/set/?set=pcb.7508973532458154&type=1"
                            },
                            "title": "Ảnh từ bài viết của Trần Văn Nhuận",
                            "type": "album",
                            "url": "https://www.facebook.com/media/set/?set=pcb.7508973532458154&type=1",
                            "subattachments": {
                                "data": [
                                    {
                                        "media": {
                                            "image": {
                                                "height": 636,
                                                "src": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-6/434996395_1368587073828864_1287516045038210399_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeG8g10UvPspuPTXUBcRyQDE8N3ClUTbLfTw3cKVRNst9FFQk0qW9-VMY-ITZ1-d6K3KmS0-spm5p_qtd2O0Vq2F&_nc_ohc=-zxUgXL3KhwAb6OlB10&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfCxwdqLBwSJpzmjcde_fDAMfdKv3Z9aPVcOtYJgrp0cnA&oe=6622B9C6",
                                                "width": 542
                                            }
                                        },
                                        "target": {
                                            "id": "1368587077162197",
                                            "url": "https://www.facebook.com/photo.php?fbid=1368587077162197&set=gm.7508973525791488&type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/photo.php?fbid=1368587077162197&set=gm.7508973525791488&type=3"
                                    },
                                    {
                                        "media": {
                                            "image": {
                                                "height": 407,
                                                "src": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-6/435010862_1368587180495520_6031326247122835027_n.jpg?_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHKS6GKcyGYcFh4p-4EcJGsutae6vGaWuG61p7q8Zpa4bcz60uha31mKed8AQg4cKOcf9Kaix4lXc57JpOxBf48&_nc_ohc=GI0-jMWurv0Ab5jERMu&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfBToj3CmdUAyQbEIlVfqoDKZIlJEEZU8K9pfn2EE04kdA&oe=6622CDA2",
                                                "width": 1028
                                            }
                                        },
                                        "target": {
                                            "id": "1368587183828853",
                                            "url": "https://www.facebook.com/photo.php?fbid=1368587183828853&set=gm.7508973529124821&type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/photo.php?fbid=1368587183828853&set=gm.7508973529124821&type=3"
                                    }
                                ]
                            }
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 8
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 9
                    }
                }
            },
            {
                "id": "1777766135578951_7492961424059365",
                "created_time": "2024-04-05T19:34:37+07:00",
                "message": "Có bạn nào bán công nghệ auto android ngay trên phone mà phải k ta",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 21
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 39
                    }
                },
                "shares": {
                    "count": 3
                }
            },
            {
                "id": "1777766135578951_7508487522506755",
                "created_time": "2024-04-09T10:50:08+07:00",
                "message": "Mình cần 1 bạn hỗ trợ hook vào vpn gate để kiểm tra khi vpn bị disconnect thì tự động connect vào luồng khác. Bạn nào làm được comment mình sẽ inbox trực tiếp ạ.",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 2
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7513452028676971",
                "created_time": "2024-04-10T15:48:16+07:00",
                "message": "code client",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 860,
                                    "src": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-6/435981690_7614537951938054_1151351611897974181_n.jpg?stp=dst-jpg_p720x720&_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeGNAHkaDbTopJrENsC_wvUioNK7ALpf_Cyg0rsAul_8LJdtdOekjl1XUXdMLISTJ_rBwbipUXIQqxPig-fnq_Wn&_nc_ohc=mHP5UkPWDyEAb5fbmsL&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfCYRANLM7oW3dJfwIQBVVZF_GrwmgbiY7kkKMW8r6neyw&oe=6622AC0C",
                                    "width": 720
                                }
                            },
                            "target": {
                                "id": "7614537965271386",
                                "url": "https://www.facebook.com/7614493831942466/photos/gm.7513452028676971/7614537965271386/?type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/7614493831942466/photos/gm.7513452028676971/7614537965271386/?type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                }
            },
            {
                "id": "1777766135578951_7508369782518529",
                "created_time": "2024-04-09T10:08:54+07:00",
                "message": "Tài chính 30M cần mua api follow tiktok bẳng request.💵💸",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 5
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                }
            },
            {
                "id": "1777766135578951_7503747526314088",
                "created_time": "2024-04-08T07:21:28+07:00",
                "message": "Xin phép ad ạ\nCác bác ơi giúp e với, e có sử dụng capture image by handle bằng hơkteam hướng dẫn, tuy nhiên khi e chụp màn hình của web site trên brave hoặc chrome thì nó ra ảnh đen, e kiểm tra bằng autoit thì nguyên trang chỉ có 2 hànle là chrome ưiget 1 và cái win d3d. K có handle con khác, các bác giúp e với",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 4
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7513452032010304",
                "created_time": "2024-04-10T15:48:16+07:00",
                "message": "Thật sự là khi gặp lỗi này em đã tìm kiếm đủ mọi cách trên mạng rồi nhưng vẫn không biết được tại sao lỗi, nhờ anh chị trong này giúp em với ạ.\nTóm tắt chương trình: em muốn làm 2 ứng dụng là sever và client chạy trên 2 máy khác nhau và kết nối với nhau bằng mạng Lan. sever mở lên, client nhập ip của sever và kết nối tới sever. Khi kết nối thành công thì ở trên máy sever nhập gì xong ấn enter, nội dung sẽ gửi đến sever, sever nhận được và gửi lại thêm câu \"Bạn đã nhập: \" . Việc này cứ diễn ra liên tục. \n\nNhưng vấn đề ỏ chỗ nếu em chạy debug cuar visual studio trên máy client thì không có lỗi gì nhưng nếu cả sever và client chạy file.exe thì bị lỗi sau: sau khi em ấn enter ở client để gửi xâu thứ nhất đi thì client không thấy nhận lại xâu đã chỉnh sửa từ sever, gõ thêm xâu thứ 2 và enter đi thì xâu thứ nhất mới gửi về. Em đang nghĩ là do phím enter vẫn còn trong bộ nhớ đệm bla bla\nDưới đây là code:",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 718,
                                    "src": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-6/435683071_7614537941938055_5601643726576226267_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEjt6LnF_LqbrLbc6wRl-zBEp_FkMTJ3LcSn8WQxMnct3FRsIpXi6M03QY6sodeCyk6uKZlFYDHW5bDzAo3MVh-&_nc_ohc=WcdkhOfro7wAb5JtTCu&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfDI2rc8jfdgleKNmj6H_RGeBA41qU1bz8I9eQq5yBcwCg&oe=6622BFEC",
                                    "width": 960
                                }
                            },
                            "target": {
                                "id": "7513452032010304",
                                "url": "https://www.facebook.com/media/set/?set=pcb.7513452032010304&type=1"
                            },
                            "title": "Ảnh từ bài viết của Người tham gia ẩn danh",
                            "type": "album",
                            "url": "https://www.facebook.com/media/set/?set=pcb.7513452032010304&type=1",
                            "subattachments": {
                                "data": [
                                    {
                                        "description": "code sever",
                                        "media": {
                                            "image": {
                                                "height": 718,
                                                "src": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-6/435683071_7614537941938055_5601643726576226267_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEjt6LnF_LqbrLbc6wRl-zBEp_FkMTJ3LcSn8WQxMnct3FRsIpXi6M03QY6sodeCyk6uKZlFYDHW5bDzAo3MVh-&_nc_ohc=WcdkhOfro7wAb5JtTCu&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfDI2rc8jfdgleKNmj6H_RGeBA41qU1bz8I9eQq5yBcwCg&oe=6622BFEC",
                                                "width": 960
                                            }
                                        },
                                        "target": {
                                            "id": "7614537958604720",
                                            "url": "https://www.facebook.com/7614493831942466/photos/gm.7513452035343637/7614537958604720/?type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/7614493831942466/photos/gm.7513452035343637/7614537958604720/?type=3"
                                    },
                                    {
                                        "description": "code client",
                                        "media": {
                                            "image": {
                                                "height": 860,
                                                "src": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-6/435981690_7614537951938054_1151351611897974181_n.jpg?stp=dst-jpg_p720x720&_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeGNAHkaDbTopJrENsC_wvUioNK7ALpf_Cyg0rsAul_8LJdtdOekjl1XUXdMLISTJ_rBwbipUXIQqxPig-fnq_Wn&_nc_ohc=mHP5UkPWDyEAb5fbmsL&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfCYRANLM7oW3dJfwIQBVVZF_GrwmgbiY7kkKMW8r6neyw&oe=6622AC0C",
                                                "width": 720
                                            }
                                        },
                                        "target": {
                                            "id": "7614537965271386",
                                            "url": "https://www.facebook.com/7614493831942466/photos/gm.7513452028676971/7614537965271386/?type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/7614493831942466/photos/gm.7513452028676971/7614537965271386/?type=3"
                                    }
                                ]
                            }
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7513319922023515",
                "created_time": "2024-04-10T15:00:31+07:00",
                "message": "Ai lm đc autu game ko ạ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                }
            },
            {
                "id": "1777766135578951_7513044918717682",
                "created_time": "2024-04-10T13:20:31+07:00",
                "message": "Cần mua mua code selenium c# giải captcha kéo thả bybit",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7484761494879358",
                "created_time": "2024-04-03T21:30:41+07:00",
                "message": "Hôm qua mình có chia sẻ cho ae tool check trạng thái và unlock acc twitter tốn rất ít CPU mà lại nhanh tại đây: https://www.facebook.com/groups/autocsharp/posts/7480776758611165/\nMà bài viết đó bị lỗi không đọc được comment của ae nên mình viết thêm bài này để chia sẻ cho ae cách sửa lại tool này để áp dụng vào hệ thống của ae.\nỞ code mình chia sẻ thì mình có\n- Tạo 100 thread (ae có thể tuỳ chỉnh ở biến MAX_THREADS) liên tục lấy account bị lock hoặc chưa rõ trạng thái ở hệ thống của ae.\n- Kiểm tra acc này có bị lock không. Nếu bị lock mà có điền api của Rockcaptcha thì unlock luôn. Xong thì gọi api vào hệ thống để cập nhật trạng thái.\nƯu điểm của code mình là ae tạo 100 thread thì chỉ khởi tạo 100 kết nối tới server (tránh quá tải). Ae nào chạy tầm vài trăm thread thì thấy không có nhiều lợi ích. Chứ chạy vài chục máy mỗi máy 100 thread thì đỡ tạo kết nối mới -> tránh quá tải hệ thống hơn nhiều.\n- Toàn bộ code của mình đều xài bất đồng bộ => Tối ưu CPU sử dụng. Máy yếu vẫn chạy tốt. Không chỉ unlock tài khoản twitter mà các tác vụ khác cần gọi lên server, gọi request ae vẫn có thể tham khảo để tối ưu tool của mình nha.\nCode mình sẽ gửi ở phần bình luận. Ae xem bài viết cũ của mình có link bên trên và đọc bình luận để lấy link nhé.\nVẫn là tiện thể ae có cần đăng ký rockcaptcha để giải twitter/outlook thì dùng link ref để ủng hộ mình viết thêm vài bài chia sẻ nữa nha.\n\nLink đăng ký rock: [https://rockcaptcha.com?affref=36411](https://rockcaptcha.com/?affref=36411&fbclid=IwAR2HIMSI8GUDAa1Zs0lX3E6cnEXbLW9UvgwGaWSODFo-KgIIDI6DCho8EhM_aem_AZRRtFRq_LMDP2gOAl-gwYGrfRePz6ZLISFBTS7aUj-9x9nopTyzFKCQg1wr9en_CJfUX7Jw1d3rfRZWyzEMAz3i)\nCảm ơn ae nhiều.",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 720,
                                    "src": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.30808-6/434669653_737824628539667_6961400536480160733_n.jpg?stp=cp1_dst-jpg_p720x720&_nc_cat=111&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeFsk6zx8usKIWDBpmyxLj9JefDwK9t26bV58PAr23bptWyuLtwPjr7ctiDrunCmte-8G22GEvqw4Ex_AekBrYlL&_nc_ohc=0JXGxhOcPmsAb5aeMqz&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfC5mgv01bbANzR2gjGe5racGl2ukcQLQPqKxuGA6MPFXw&oe=6622CC5F",
                                    "width": 1230
                                }
                            },
                            "target": {
                                "id": "737824631873000",
                                "url": "https://www.facebook.com/photo.php?fbid=737824631873000&set=gm.7484761494879358&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=737824631873000&set=gm.7484761494879358&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 13
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 54
                    }
                },
                "shares": {
                    "count": 6
                }
            },
            {
                "id": "1777766135578951_7511974675491373",
                "created_time": "2024-04-10T07:02:06+07:00",
                "message": "Bác nào bán phone info để fake thông số điện thoại thì chấm cái ở dưới bài này để e ib nhé.",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 6
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                }
            },
            {
                "id": "1777766135578951_7509580485730792",
                "created_time": "2024-04-09T17:35:57+07:00",
                "message": "Em có acc facebook dính checkpoint, có cách nào lấy được full name của acc không ? các bác giúp đỡ em cám ơn ạ.",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 4
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7503992629622911",
                "created_time": "2024-04-08T08:49:11+07:00",
                "message": "Cần 1 ban train C# cơ bản http và winform",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 6
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 4
                    }
                }
            },
            {
                "id": "1777766135578951_7470820119606829",
                "created_time": "2024-03-31T15:28:55+07:00",
                "message": "#hoidap **Cần mua cách backup restore google Account trên Android + change info full cho android**",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 5
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 5
                    }
                }
            },
            {
                "id": "1777766135578951_7501826256506215",
                "created_time": "2024-04-07T20:12:48+07:00",
                "message": "Có bác nào bán source python về tool làm video đọc truyện tranh không. Mình đang hứng thú cần mua vọc vạch",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 2
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 9
                    }
                }
            },
            {
                "id": "1777766135578951_7506364972719010",
                "created_time": "2024-04-08T23:01:13+07:00",
                "message": "Hiện em đang bị mắc chỗ mở LD, mỗi máy tốc độ mở LD khác nhau. Các bác có cách nào check đc khi nó mở xong ko ạ. (Opened not Running)",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 513,
                                    "src": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-6/435417153_122130359774222326_8789777176492664706_n.jpg?_nc_cat=103&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeGi5LfktI0K9-UzfSbLd9UR2sNzpA9KwAHaw3OkD0rAAfKMYud-rH3ADgEtEb0JHi0LVKLWpEj6QV-2b8fe6ndE&_nc_ohc=RdWJB9oZfoYAb5lzSCB&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfCTNjR9eSLehQCxC3XH2U8yBFOM4coHDDWGt3vvGPoBCQ&oe=6622CF65",
                                    "width": 321
                                }
                            },
                            "target": {
                                "id": "122130359780222326",
                                "url": "https://www.facebook.com/photo.php?fbid=122130359780222326&set=gm.7506364972719010&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=122130359780222326&set=gm.7506364972719010&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7505170862838421",
                "created_time": "2024-04-08T16:19:52+07:00",
                "message": "Chào mọi người, mình cần 1 bạn cài và chạy giúp mình 1 project web C# ạ. Có hậu tạ ạ, cảm ơn!",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 720,
                                    "src": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.30808-6/434950319_429806476266124_9001583768201269052_n.png?stp=dst-png_p720x720&_nc_cat=108&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeFiWGbbydgNTaeDVGH80HUYzxVHMAVxmzrPFUcwBXGbOhr7GEcoMyaTFFLXYN-DztSeTZkgnWzDurLxQqMIJywz&_nc_ohc=CZrbrakgXgQAb6qa4A5&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfBJaj8C5Ox-kW4IA_t8CNJ8VZLXbClaNLNdllvlx__etQ&oe=6622B901",
                                    "width": 1280
                                }
                            },
                            "target": {
                                "id": "429806479599457",
                                "url": "https://www.facebook.com/429805846266187/photos/gm.7505170862838421/429806479599457/?type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/429805846266187/photos/gm.7505170862838421/429806479599457/?type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7506004939421680",
                "created_time": "2024-04-08T21:10:47+07:00",
                "message": "Có bác nào từng làm tool quản lí metamask full request hoặc tương tự vậy chưa ạ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 7
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 9
                    }
                }
            },
            {
                "id": "1777766135578951_7505182016170639",
                "created_time": "2024-04-08T16:24:16+07:00",
                "message": "mình cần 1 bạn viết tool hoạt động cùng lúc trên nhiều tab chrome ở thủ đức ai chuyên viết tool thì cmt mình chủ động nhắn nhé",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 4
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7508744605814380",
                "created_time": "2024-04-09T12:22:59+07:00",
                "message": "Cần 1 bạn code extension nhấn vào một chỗ trên web ai làm inb",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                }
            },
            {
                "id": "1777766135578951_7508311669191007",
                "created_time": "2024-04-09T09:48:49+07:00",
                "message": "Em cần học code để code auto lấy otp trên bank androind hoặc ios có ai dạy không ạ hoặc cho em từ khoá tìm hiểu cách với",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 2
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 6
                    }
                }
            },
            {
                "id": "1777766135578951_7505665702788937",
                "created_time": "2024-04-08T19:17:33+07:00",
                "message": "E cần 1 tool edit video nhanh gọn lẹ như sau ạ\nInput video vào video dọc\nOutput ra là dọc nhưng có viền đen xung quanh, với viền đen chia đôi video ra ạ như ví dụ dưới",
                "attachments": {
                    "data": [
                        {
                            "target": {
                                "id": "7505665702788937",
                                "url": "https://www.facebook.com/media/set/?set=pcb.7505665702788937&type=1"
                            },
                            "title": "Ảnh từ bài viết của Duy Van Pham",
                            "type": "album",
                            "url": "https://www.facebook.com/media/set/?set=pcb.7505665702788937&type=1",
                            "subattachments": {
                                "data": [
                                    {
                                        "media": {
                                            "image": {
                                                "height": 720,
                                                "src": "https://scontent.fsgn2-4.fna.fbcdn.net/v/t15.5256-10/431412594_966443558533259_5614607594380914662_n.jpg?stp=dst-jpg_s720x720&_nc_cat=101&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeGyhSECwBsV23EtJVWGKTm4dZ9eEfniO8F1n14R-eI7wQhV0EdcvpcH-MsyHsAudSizNoAIIIfoaqnzLTfx_j8i&_nc_ohc=KqAhrOwIR9wAb7x3vPR&_nc_ht=scontent.fsgn2-4.fna&oh=00_AfACuLjEdhtsTL8BHZ-Wu2T6M6T8qBjCVk--9BN55356Aw&oe=6622B6D6",
                                                "width": 405
                                            },
                                            "source": "https://scontent.fsgn2-11.fna.fbcdn.net/o1/v/t2/f1/m69/GEN_CBoQBylmO3MDAJb67aWkM9QUbmdjAAAF.mp4?efg=eyJ2ZW5jb2RlX3RhZyI6Im9lcF9oZCJ9&_nc_ht=scontent.fsgn2-11.fna.fbcdn.net&_nc_cat=104&_nc_eui2=AeHzcF4uqwEZ2epv2jXhnC2GhCXQ4TYT5-SEJdDhNhPn5DqHBq-jLSInzNwljIb2ruJ_KvdzY9fCwws8TKtIOOZY&strext=1&vs=c3b35f258f26ea47&_nc_vs=HBksFQIYOnBhc3N0aHJvdWdoX2V2ZXJzdG9yZS9HRU5fQ0JvUUJ5bG1PM01EQUpiNjdhV2tNOVFVYm1kakFBQUYVAALIAQAVAhg6cGFzc3Rocm91Z2hfZXZlcnN0b3JlL0dEamotUm4xeG1zTzRzb0NBRjJtSnoyY1RfQkRidjRHQUFBRhUCAsgBAEsHiBJwcm9ncmVzc2l2ZV9yZWNpcGUBMQ1zdWJzYW1wbGVfZnBzABB2bWFmX2VuYWJsZV9uc3ViACBtZWFzdXJlX29yaWdpbmFsX3Jlc29sdXRpb25fc3NpbQAoY29tcHV0ZV9zc2ltX29ubHlfYXRfb3JpZ2luYWxfcmVzb2x1dGlvbgAddXNlX2xhbmN6b3NfZm9yX3ZxbV91cHNjYWxpbmcAEWRpc2FibGVfcG9zdF9wdnFzABUAJQAcjBdAAAAAAAAAABERAAAAJoz76fiIh7QDFQIoAkMzGAt2dHNfcHJldmlldxwXQBAAAAAAAAAYIWRhc2hfZ2VuMmh3YmFzaWNfaHEyX2ZyYWdfMl92aWRlbxIAGBh2aWRlb3MudnRzLmNhbGxiYWNrLnByb2Q4ElZJREVPX1ZJRVdfUkVRVUVTVBsKiBVvZW1fdGFyZ2V0X2VuY29kZV90YWcGb2VwX2hkE29lbV9yZXF1ZXN0X3RpbWVfbXMBMAxvZW1fY2ZnX3J1bGUHdW5tdXRlZBNvZW1fcm9pX3JlYWNoX2NvdW50BTI5OTA5EW9lbV9pc19leHBlcmltZW50AAxvZW1fdmlkZW9faWQQMjE0MTc2ODU5MjgzMTMxNxJvZW1fdmlkZW9fYXNzZXRfaWQPNDUzMTA2NzMwNTYwMzUwFW9lbV92aWRlb19yZXNvdXJjZV9pZA85NTg4OTU1OTg5NDM5NDIcb2VtX3NvdXJjZV92aWRlb19lbmNvZGluZ19pZA85NjcwNDUzODgyNjM0OTIOdnRzX3JlcXVlc3RfaWQAJQIcACXEARsHiAFzBDYzODgCY2QKMjAyNC0wNC0wOANyY2IFMjk5MDADYXBwE0ZhY2Vib29rIGZvciBpUGhvbmUCY3QKR1JPVVBfUE9TVBNvcmlnaW5hbF9kdXJhdGlvbl9zATQCdHMVcHJvZ3Jlc3NpdmVfZW5jb2RpbmdzAA%3D%3D&ccb=9-4&oh=00_AfAFrqyQ-trxWftKcnNEAIiYAF_5sMu0VjJEZbi5v2VRsA&oe=661EC5BD&_nc_sid=1d576d&_nc_rid=249992122048916&_nc_store_type=1"
                                        },
                                        "target": {
                                            "id": "2141768592831317",
                                            "url": "https://www.facebook.com/groups/autocsharp/permalink/7505665702788937/"
                                        },
                                        "type": "video_autoplay",
                                        "url": "https://www.facebook.com/groups/autocsharp/permalink/7505665702788937/"
                                    },
                                    {
                                        "media": {
                                            "image": {
                                                "height": 720,
                                                "src": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t15.5256-10/431805042_796179815247741_3339188636384621147_n.jpg?stp=dst-jpg_s720x720&_nc_cat=105&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeHBZTQvg73skBCGxneD3S9AtAaIEuGOkvi0BogS4Y6S-GN8h8s2fKOALUGc01k3BlkEkYuLEkoqG4fi1WMbYsI2&_nc_ohc=_IQvt1l75EoAb4nKy_P&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfAp0ShJyUHSU9zqUt2eotoQrR1mmnn58s2mW5b3QAdg2A&oe=6622AF21",
                                                "width": 405
                                            },
                                            "source": "https://scontent.fsgn2-11.fna.fbcdn.net/o1/v/t2/f1/m69/GLvZ7hlmyC7P8IECALfbR4WW5SkHbmdjAAAF.mp4?efg=eyJ2ZW5jb2RlX3RhZyI6Im9lcF9oZCJ9&_nc_ht=scontent.fsgn2-11.fna.fbcdn.net&_nc_cat=110&_nc_eui2=AeGA3IyQNs7HlKBBt4ymHljysfgCBEQAUuOx-AIERABS41OSB14YUAqgQnOdx5PEkaV24YLK_4b3NSeSg-Ln3QpT&strext=1&vs=3805518c184268e8&_nc_vs=HBksFQIYOnBhc3N0aHJvdWdoX2V2ZXJzdG9yZS9HTHZaN2hsbXlDN1A4SUVDQUxmYlI0V1c1U2tIYm1kakFBQUYVAALIAQAVAhg6cGFzc3Rocm91Z2hfZXZlcnN0b3JlL0dBN3JBeHFrUEJVTVpwSUZBRTBDU21XTkhMVmdidjRHQUFBRhUCAsgBAEsHiBJwcm9ncmVzc2l2ZV9yZWNpcGUBMQ1zdWJzYW1wbGVfZnBzABB2bWFmX2VuYWJsZV9uc3ViACBtZWFzdXJlX29yaWdpbmFsX3Jlc29sdXRpb25fc3NpbQAoY29tcHV0ZV9zc2ltX29ubHlfYXRfb3JpZ2luYWxfcmVzb2x1dGlvbgAddXNlX2xhbmN6b3NfZm9yX3ZxbV91cHNjYWxpbmcAEWRpc2FibGVfcG9zdF9wdnFzABUAJQAcjBdAAAAAAAAAABERAAAAJu7nvc3MvbQBFQIoAkMzGAt2dHNfcHJldmlldxwXQBAAAAAAAAAYIWRhc2hfZ2VuMmh3YmFzaWNfaHEyX2ZyYWdfMl92aWRlbxIAGBh2aWRlb3MudnRzLmNhbGxiYWNrLnByb2Q4ElZJREVPX1ZJRVdfUkVRVUVTVBsKiBVvZW1fdGFyZ2V0X2VuY29kZV90YWcGb2VwX2hkE29lbV9yZXF1ZXN0X3RpbWVfbXMBMAxvZW1fY2ZnX3J1bGUHdW5tdXRlZBNvZW1fcm9pX3JlYWNoX2NvdW50BTI5OTA5EW9lbV9pc19leHBlcmltZW50AAxvZW1fdmlkZW9faWQPNzE3MDc1MTgwNTA2ODMwEm9lbV92aWRlb19hc3NldF9pZBAxMTM4NjExODIzOTM4OTIwFW9lbV92aWRlb19yZXNvdXJjZV9pZA8zOTY4ODI0Mzk4MTM2MjMcb2VtX3NvdXJjZV92aWRlb19lbmNvZGluZ19pZA8zNzg0MzkzNTgzNTEwNjgOdnRzX3JlcXVlc3RfaWQAJQIcACXEARsHiAFzBDg4NjkCY2QKMjAyNC0wNC0wOANyY2IFMjk5MDADYXBwE0ZhY2Vib29rIGZvciBpUGhvbmUCY3QKR1JPVVBfUE9TVBNvcmlnaW5hbF9kdXJhdGlvbl9zATQCdHMVcHJvZ3Jlc3NpdmVfZW5jb2RpbmdzAA%3D%3D&ccb=9-4&oh=00_AfC41QZB2korszSYq1zSPno7w7nWVC8ibYsMzDR42YmU_w&oe=661EC3AA&_nc_sid=1d576d&_nc_rid=005790082211515&_nc_store_type=1"
                                        },
                                        "target": {
                                            "id": "717075180506830",
                                            "url": "https://www.facebook.com/groups/autocsharp/permalink/7505665702788937/"
                                        },
                                        "type": "video_autoplay",
                                        "url": "https://www.facebook.com/groups/autocsharp/permalink/7505665702788937/"
                                    }
                                ]
                            }
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 6
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7502255196463321",
                "created_time": "2024-04-07T22:32:13+07:00",
                "message": "Cùng là 1 profile chrome nhưng khi em mở qua tool người khác thì thông số hardware của trình profile khác nhau còn khi mở qua selenium c# thì thông số đó vẫn giữ nguyên (mở bất kỳ profile nào cũng vậy không thay đổi). Các bác cho e hỏi e có đang sai ở đâu không ạ? (ảnh 1 bên trái là mở bằng tool khác, ảnh 1 bên phải là mở bằng selenium e tự code) \n   Ngoài ra thì để nuôi acc x, fb, tt thì thông số hardware trùng nhau có ảnh hưởng gì không khi trình duyệt được tick xanh \"Trustworthy\" của iphey (ảnh 2)",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 720,
                                    "src": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-6/434684870_3806992272882098_1150104324795489163_n.jpg?stp=dst-jpg_p720x720&_nc_cat=106&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeErMHXKz9iI2RrEnNbqEXwROS4Owtz7mYc5Lg7C3PuZh4LsmXl8IbgQLn9Dxy99-zoApps5AaIw--IVjhX-5c5A&_nc_ohc=LqTXUfcm0KEAb48mszX&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfBFLavJuq0ewDOxQBuFCxWsDfeL-w7iOs-rc4k51M3VdQ&oe=6622D3E5",
                                    "width": 1280
                                }
                            },
                            "target": {
                                "id": "7502255196463321",
                                "url": "https://www.facebook.com/media/set/?set=pcb.7502255196463321&type=1"
                            },
                            "title": "Ảnh từ bài viết của Phạm Hoàng Hiệp",
                            "type": "album",
                            "url": "https://www.facebook.com/media/set/?set=pcb.7502255196463321&type=1",
                            "subattachments": {
                                "data": [
                                    {
                                        "media": {
                                            "image": {
                                                "height": 720,
                                                "src": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-6/434684870_3806992272882098_1150104324795489163_n.jpg?stp=dst-jpg_p720x720&_nc_cat=106&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeErMHXKz9iI2RrEnNbqEXwROS4Owtz7mYc5Lg7C3PuZh4LsmXl8IbgQLn9Dxy99-zoApps5AaIw--IVjhX-5c5A&_nc_ohc=LqTXUfcm0KEAb48mszX&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfBFLavJuq0ewDOxQBuFCxWsDfeL-w7iOs-rc4k51M3VdQ&oe=6622D3E5",
                                                "width": 1280
                                            }
                                        },
                                        "target": {
                                            "id": "3806992276215431",
                                            "url": "https://www.facebook.com/photo.php?fbid=3806992276215431&set=gm.7502255189796655&type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/photo.php?fbid=3806992276215431&set=gm.7502255189796655&type=3"
                                    },
                                    {
                                        "media": {
                                            "image": {
                                                "height": 663,
                                                "src": "https://scontent.fsgn2-9.fna.fbcdn.net/v/t39.30808-6/423715197_3806994289548563_6703473397341257009_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeFIPUXFufWV6Btg-ejZ1vC9uqQ1yHS9uEO6pDXIdL24Q_XXfV9gM1ky5Il0Ue1GGI7VW9g_ncr0v3ytNuEv54ro&_nc_ohc=D9CatI6s_r4Ab4DgSgX&_nc_ht=scontent.fsgn2-9.fna&oh=00_AfCcVOZvKshG_xAZLIst0IjAhRwb0zWOE1Nj2tLQUdChAg&oe=6622A595",
                                                "width": 1165
                                            }
                                        },
                                        "target": {
                                            "id": "3806994296215229",
                                            "url": "https://www.facebook.com/photo.php?fbid=3806994296215229&set=gm.7502255193129988&type=3"
                                        },
                                        "type": "photo",
                                        "url": "https://www.facebook.com/photo.php?fbid=3806994296215229&set=gm.7502255193129988&type=3"
                                    }
                                ]
                            }
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 8
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 7
                    }
                },
                "shares": {
                    "count": 2
                }
            },
            {
                "id": "1777766135578951_7493139537374887",
                "created_time": "2024-04-05T20:25:45+07:00",
                "message": "anh chị nào còn hay có link download đoạn code AddLDPlayerToWPF của anh Long không cho em xin nha. Em cảm ơn anh chị🙏😁😅🙏",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                }
            },
            {
                "id": "1777766135578951_7505213729500801",
                "created_time": "2024-04-08T16:35:46+07:00",
                "message": "Mn cho e hỏi\nBị lỗi như hình dưới mặc dù e đã thêm vào references Gam.BaseViewModel và trong class đã có using Gam.BaseViewModel;",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 33,
                                    "src": "https://scontent.fsgn2-10.fna.fbcdn.net/v/t39.30808-6/435082552_3615045898760749_5900716870862702420_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeFMYxbNrhX6A4XZtIJKPsjuIbH9EYHacvYhsf0Rgdpy9gmAVfTg-6zRlIqN5YaCfQ0pcWay5EhLH2nJoP-fXWee&_nc_ohc=SVPL3lEaWUAAb4-cOOZ&_nc_ht=scontent.fsgn2-10.fna&oh=00_AfCZtRTyhK9S4qF7l_QCrokV0VQxGbdzdX5_WI2U8GPihQ&oe=6622BC6F",
                                    "width": 384
                                }
                            },
                            "target": {
                                "id": "3615045902094082",
                                "url": "https://www.facebook.com/photo.php?fbid=3615045902094082&set=gm.7505213729500801&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=3615045902094082&set=gm.7505213729500801&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 2
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                }
            },
            {
                "id": "1777766135578951_7504898882865619",
                "created_time": "2024-04-08T14:34:51+07:00",
                "message": "Các cao nhân ai biết chỉ e với!",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 720,
                                    "src": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.30808-6/435310662_3636624806584135_8277529577286283731_n.jpg?stp=dst-jpg_p720x720&_nc_cat=111&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeFVwZqoIHjaOoX-ejMaUwDBwPp0h4enu7bA-nSHh6e7thpLasUzRRAL4BO1Z-Hm0C3So9sdEIfgLvbstnJJyWp4&_nc_ohc=gvWqp0glob0Ab4qR-42&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfBRL96eoeO2QZuUKv9LLqf1w2d-_58RvgrmqrmfWau8dQ&oe=6622D492",
                                    "width": 958
                                }
                            },
                            "target": {
                                "id": "3636624809917468",
                                "url": "https://www.facebook.com/1413512862722063/photos/gm.7504898882865619/3636624809917468/?type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/1413512862722063/photos/gm.7504898882865619/3636624809917468/?type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                }
            },
            {
                "id": "1777766135578951_7503729819649192",
                "created_time": "2024-04-08T07:14:06+07:00",
                "message": "Thấy Gr này mn rất hay chia sẻ kinh nghiệm coder. E mới tập code python k biết cách fake trình duyệt xịn bác nào có thể chia sẻ ít tài liệu, thư viện tạo và thao tác trên trình duyệt ko ạ. Và e cần 1 công cụ kiểm thử MATH, CSS, Xpath, vị trí trên web. Như kiểu android có adb capture của howkteam ấy",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 4
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                }
            },
            {
                "id": "1777766135578951_7492769214078586",
                "created_time": "2024-04-05T18:36:39+07:00",
                "message": "Cần một bạn biết bắt api trên app về team ae cùng chinh chiến ạ.",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 7
                    }
                }
            },
            {
                "id": "1777766135578951_7501443423211165",
                "created_time": "2024-04-07T18:00:47+07:00",
                "message": "Có cách nào tắt cảm biến xoay trên android ko các bác , lật ngang boxphone vô app fb là nó tự xoay . Tắt trong cài đặt change device cái trở về như cũ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 2
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7501187273236780",
                "created_time": "2024-04-07T16:27:26+07:00",
                "message": "e đang làm tool sử dụng thư viện threading để chạy mà có lúc chạy không bị sót tài khoản, bác nào nhận fix lỗi này ib e với e gửi ly cafe",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 175,
                                    "src": "https://scontent.fsgn2-6.fna.fbcdn.net/v/t39.30808-6/435108101_1064449428433435_1116108374065508855_n.png?_nc_cat=110&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeESK7ghp33A78EJGEnk-w2N5eEVpc0ctkXl4RWlzRy2RZZbp47w9PaFhDM8Igf4Gu9ui62FZpcHeaRGekkPSeqY&_nc_ohc=eInCCJlor2EAb5KTJyZ&_nc_ht=scontent.fsgn2-6.fna&oh=00_AfAEBYESSgRRTrofVqbdWjAAjBisAG6W7J9gZUU_dk97nw&oe=6622D5C7",
                                    "width": 1339
                                }
                            },
                            "target": {
                                "id": "1064449431766768",
                                "url": "https://www.facebook.com/781674856710895/photos/gm.7501187273236780/1064449431766768/?type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/781674856710895/photos/gm.7501187273236780/1064449431766768/?type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 2
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 3
                    }
                }
            },
            {
                "id": "1777766135578951_7502627473092760",
                "created_time": "2024-04-08T00:37:21+07:00",
                "message": "Có bác nào code ASP.NetCore trên ubuntu chưa ạ cho e xin chút thông tin ạ về IDE, có phù hợp để code multiplatform không ạ, tại e thấy nó khá mượt :v và nhẹ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 4
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 4
                    }
                }
            },
            {
                "id": "1777766135578951_7501286389893535",
                "created_time": "2024-04-07T17:02:59+07:00",
                "message": "Em đang thử mày mò chỗ giải recapchav3 mà chưa biết dùng như nào ai chỉ em với được không ạ có api nào free để test thử hay có chỗ nào rẻ rẻ để thử không ạ em cám ơn anh chị ạ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 43
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                }
            },
            {
                "id": "1777766135578951_7502398849782289",
                "created_time": "2024-04-07T23:20:13+07:00",
                "message": "Các bác có thể chia sẻ giúp em api facebook để search các bài post trong 1 page theo từ khóa được không ạ. Em ngồi đọc document trên facebook mà tìm mãi không ra rồi ạ.😁",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 0
                    }
                }
            },
            {
                "id": "1777766135578951_7498114590210715",
                "created_time": "2024-04-06T22:53:01+07:00",
                "message": "ai nhận làm app quản lý siêu thị vài chức năng đơn giản bằng c# ko ạ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 13
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 10
                    }
                }
            },
            {
                "id": "1777766135578951_7204978066191037",
                "created_time": "2024-01-24T21:25:28+07:00",
                "message": "bên mình vừa build server giải recaptcha v3, ai cần ib mình có site demo",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 720,
                                    "src": "https://scontent.fsgn2-7.fna.fbcdn.net/v/t39.30808-6/421205771_2118281135190897_7394289378138332818_n.jpg?stp=dst-jpg_p720x720&_nc_cat=100&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeGTTUDOGennIISycqY_2Cvr5rojyOG8dgTmuiPI4bx2BP0oUxccYsd8kGXKudCDUV-6W3nPxj2k3jPrGs0yLTAI&_nc_ohc=npQ-2XoJgeAAb5g_Tr-&_nc_ht=scontent.fsgn2-7.fna&oh=00_AfAjlHS0Hj5L-bQoBrjiDlnLj2WtVpg_b5McvolrCyRviw&oe=6622B84F",
                                    "width": 1206
                                }
                            },
                            "target": {
                                "id": "2118281138524230",
                                "url": "https://www.facebook.com/photo.php?fbid=2118281138524230&set=gm.7204978066191037&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=2118281138524230&set=gm.7204978066191037&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 9
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 26
                    }
                },
                "shares": {
                    "count": 1
                }
            },
            {
                "id": "1777766135578951_6715948931760622",
                "created_time": "2023-09-14T16:03:14+07:00",
                "message": "Mình cần login facebook bằng request sử dụng cookie, ae nào bik ko ạ",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 10
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 5
                    }
                },
                "shares": {
                    "count": 1
                }
            },
            {
                "id": "1777766135578951_7500301363325371",
                "created_time": "2024-04-07T11:06:42+07:00",
                "message": "Dạ e chào mọi người, e có thể hỏi entity framework là gì không ạ? Do e có tìm hiểu nhưng vẫn chưa thật sự hiểu, với cả có những nguồn nào để em có thể tự học được ạ, em cảm ơn.",
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 1
                    }
                }
            },
            {
                "id": "1777766135578951_7500256676663173",
                "created_time": "2024-04-07T10:51:54+07:00",
                "message": "Nếu em mở 2 profile cùng 1 lúc thì em dùng Image Search (Kautohelper) để Click vào ô Captcha như thế nào ạ? Nếu 1 profile thì nhận diện tọa độ của 1 cái nó dễ hơn. Có cách nào chỉ chụp màn hình của 1 profile không ạ? Hoặc bro nào có cách để vượt Captcha này mà ko cần dùng API captcha không ạ? Thanks\n#kautohelper #captcha",
                "attachments": {
                    "data": [
                        {
                            "media": {
                                "image": {
                                    "height": 188,
                                    "src": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t39.30808-6/435010799_392934373542156_963659077105189125_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEpH_w3lEdGbiSdcJmcOcM1ipNIhNiVT1GKk0iE2JVPUdhOfapLOeF8dU_iX4ANL1uRzJt9WFLXOW9YHOWLI4iP&_nc_ohc=VtwaYT02_TUAb6UkzWE&_nc_oc=Adh4G4zksMa4bwN7fGdFbgCAOGI27gODqH5-mlIll4LfPyRxSkuou5pVlhlW-TFfbKE&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfBbPF57a6L5hQI7ei9_K6PnJd9rCBZwvPR6IVMdazNNLw&oe=6622B658",
                                    "width": 1001
                                }
                            },
                            "target": {
                                "id": "392934376875489",
                                "url": "https://www.facebook.com/photo.php?fbid=392934376875489&set=gm.7500256676663173&type=3"
                            },
                            "type": "photo",
                            "url": "https://www.facebook.com/photo.php?fbid=392934376875489&set=gm.7500256676663173&type=3"
                        }
                    ]
                },
                "comments": {
                    "data": [],
                    "summary": {
                        "total_count": 2
                    }
                },
                "reactions": {
                    "data": [],
                    "summary": {
                        "total_count": 4
                    }
                }
            }
        ],
        "paging": {
            "previous": "http://graph.scanfb.top/graph/v19.0/1777766135578951/feed?access_token=N8o3eySfREuw1pbt3fmcLg&pretty=1&fields=from%2Cid%2Ccreated_time%2Cmessage%2Cattachments%7Bmedia%2Ctarget%2Ctitle%2Ctype%2Curl%2Csubattachments.limit%28100%29%7D%2Ccomments.summary%28total_count%29.limit%280%29%2Creactions.summary%28total_count%29.limit%280%29%2Cshares&__previous=1&since=1713169287&until&__paging_token=enc_AdDvYwSJXcAHdZACzcicZCsCDx87F9BrC1bY7Cva6pAJfBZCWTLq8eXk2mG8zG9oLyVhH7oHpkvz0FT15qmxZCXg66buSRZCGuVF4FXLxjr0JtTvpdQZDZD",
            "next": "http://graph.scanfb.top/graph/v19.0/1777766135578951/feed?access_token=N8o3eySfREuw1pbt3fmcLg&pretty=1&fields=from%2Cid%2Ccreated_time%2Cmessage%2Cattachments%7Bmedia%2Ctarget%2Ctitle%2Ctype%2Curl%2Csubattachments.limit%28100%29%7D%2Ccomments.summary%28total_count%29.limit%280%29%2Creactions.summary%28total_count%29.limit%280%29%2Cshares&until=1712473731&since&__paging_token=enc_AdCgavqFB1YGbr1HhvqG56cMjMLQp2c66LAcmmCqt8CvMpnE8SPNUZARccVCpds4I26fxc5z2ajh1RQCL02PZCdNeZAeiJDDP7xoqLodUrFV0MBLAZDZD&__previous"
        }
    }
}
```
</details>
