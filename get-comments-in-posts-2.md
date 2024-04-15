# APIs-Facebook-no-cookie-token
API lấy data facebook không cần dùng cookie hay token
HOÀN TOÀN MIỄN PHÍ

<details>

<summary>Get danh sách comment của bài viết (GraphQL)</summary>


```http
GET http://graph.scanfb.top/graphql/?action=post_comments&post_id=7527887927233381&cursor=&access_token=N8o3eySfREuw1pbt3fmcLg
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `post_id` | `string` | **Bắt buộc**. ID bài viết, dạng số, không có dấu '_' |
| `cursor` | `string` | Paginate |
| `access_token` | `string` | **Bắt buộc**. Token trên được chia sẽ công khai, nhiều người dùng, request có thể sẽ chậm. Liên hệ Kiệt để nhận Token riêng miễn phí |


### Response

```json
{
    "success": true,
    "message": "",
    "data": {
        "data": {
            "node": {
                "__typename": "Feedback",
                "id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MQ==",
                "should_always_show_composer_on_top": false,
                "total_comment_count": 4,
                "comment_rendering_instance_for_feed_location": {
                    "selected_intent": {
                        "intent_token": "CHRONOLOGICAL_UNFILTERED_INTENT_V1"
                    },
                    "comments": {
                        "created_comment_insertion_position": "BOTTOM",
                        "filtering_footer_string": "",
                        "count": 4,
                        "page_size": 50,
                        "total_count": 4,
                        "edges": [
                            {
                                "node": {
                                    "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1Mjc4ODg0MjA1NjY2NjU=",
                                    "feedback": {
                                        "id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTI3ODg4NDIwNTY2NjY1",
                                        "expansion_info": {
                                            "expansion_token": "MjoxNzEzMTcxMTYwOgF1dlbqXIag2yR2bQKqfi3zJsXqy1NqfQISODdFpjkrBrjEVP-F_BoQTHEoYPiY2xWa3ehJdPZ56VV21l3RKO19iPmIRLEC8wrOgbxONaWOoz2MCja525U_Q60bx3A021RnrxyaB7VOH_VIJkNM0sOZu2NOwMrsO08Y2Dirr2C4-3e-eZRJZ4z0krr1QJVhUSngFlAWmKMB0IX60hZ0-AMyhF8BMDzzU1_QoPYYBdTfwq_W9bBVBf86cpB-LPD2mP8Tzaap0S01NOYdgCJveq5WflKBmy7HRD-9M6VLjjf0HzUGsXAD-7TfgcLFdErepOTKqqSKFXLgaJs9iWUxB3nKLpmQ1RmFeUwpN86sLeofKfYJxyEUWtDgrwzUrBIigh4GywP7bjLb0FlgW6h4gtSt-bCnT98MxiFZ_IaOFSwLEGEqURE--1Nkj0D9BwK1DUo30KTMod7euqOl1M_f6YCIPY8oxF1LMz5YXIo1rrAuIb4UIO0FZXuiojQf0as0d5peZ89zmMJ8XYpKgmQ",
                                            "should_show_reply_count": true
                                        },
                                        "replies_fields": {
                                            "filtering_footer_string": "",
                                            "count": 0,
                                            "total_count": 0
                                        },
                                        "viewer_actor": {
                                            "__typename": "User",
                                            "id": "61557504676830",
                                            "__isActor": "User",
                                            "name": "Lý Mai",
                                            "profile_picture_depth_0": {
                                                "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t1.30497-1/143086968_2856368904622192_1959732218791162458_n.png?stp=cp0_dst-png_p48x48&_nc_cat=1&ccb=1-7&_nc_sid=5f2048&_nc_ohc=kNSgHQLZ6doAb7eTDui&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDEoIPJUkx_mGovM_J3326vyBlc9auyJo-PJ_EBTtGgRg&oe=66445C78"
                                            },
                                            "profile_picture_depth_1": {
                                                "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t1.30497-1/143086968_2856368904622192_1959732218791162458_n.png?stp=cp0_dst-png_p40x40&_nc_cat=1&ccb=1-7&_nc_sid=5f2048&_nc_ohc=kNSgHQLZ6doAb7eTDui&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDqYKF91_-oKl07Nqn6ibjv0dysE8eyQkwL7oXXxsmLDA&oe=66445C78"
                                            },
                                            "gender": "MALE"
                                        },
                                        "url": "https://www.facebook.com/groups/autocsharp/posts/7527887927233381/?comment_id=7527888420566665",
                                        "__typename": "Feedback",
                                        "plugins": [
                                            {
                                                "__typename": "CommentComposerGroupMentionsPlugin",
                                                "group_id": "1777766135578951",
                                                "post_id": "7527888420566665",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerGroupMentionsPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerGroupMentionsPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerAvatarPlugin",
                                                "has_avatar": false,
                                                "feedback_id": "7527888420566665",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerAvatarPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerAvatarPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerHashtagPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerHashtagPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerHashtagPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerEmojiPlugin",
                                                "emoji_size": 16,
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerEmojiPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerEmojiPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerMediaUploadPlugin",
                                                "viewer_actor": {
                                                    "__typename": "User",
                                                    "id": "61557504676830"
                                                },
                                                "should_condense_video_preview": true,
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerMediaUploadPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerMediaUploadPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerGIFPlugin",
                                                "feedback_id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTI3ODg4NDIwNTY2NjY1",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerGIFPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerGIFPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CometComposerCometizedStickersPlugin",
                                                "feedback_id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTI3ODg4NDIwNTY2NjY1",
                                                "owning_profile_id": "100081953824049",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerStickersPlugin_next_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerStickersPlugin.next"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerEmoticonPlugin",
                                                "emoji_size": 16,
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerEmoticonPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerEmoticonPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerPrefillMentionPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerPrefillMentionPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerPrefillMentionPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerAssociateReplyWithParentPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerAssociateReplyWithParentPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerAssociateReplyWithParentPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerSetReplyClickedPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerSetReplyClickedPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerSetReplyClickedPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerStateSnapshotPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerStateSnapshotPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerStateSnapshotPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerLiveTypingBroadcastPlugin",
                                                "feedback_id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTI3ODg4NDIwNTY2NjY1",
                                                "viewer_actor": {
                                                    "__typename": "User",
                                                    "id": "61557504676830"
                                                },
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerLiveTypingBroadcastPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerLiveTypingBroadcastPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerCommentCharacterLimitPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerCommentCharacterLimitPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerCommentCharacterLimitPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerWriteToComposerPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerWriteToComposerPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerWriteToComposerPlugin"
                                                }
                                            }
                                        ],
                                        "comment_composer_placeholder": "Viết phản hồi công khai…",
                                        "can_viewer_comment": true,
                                        "constituent_badge_banner_renderer": null,
                                        "have_comments_been_disabled": false,
                                        "are_live_video_comments_disabled": false,
                                        "is_viewer_muted": false,
                                        "total_comment_count": 0,
                                        "comments_disabled_notice_renderer": {
                                            "__typename": "GeneralCommentDisableNotice",
                                            "notice_message": {
                                                "delight_ranges": [],
                                                "image_ranges": [],
                                                "inline_style_ranges": [],
                                                "aggregated_ranges": [],
                                                "ranges": [],
                                                "color_ranges": [],
                                                "text": "Bình luận đã bị tắt cho bài viết này."
                                            },
                                            "__module_operation_CometUFICommentDisabledNotice_feedback": {
                                                "__dr": "CometGenericCommentDisableNotice_commentDisableNotice$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentDisabledNotice_feedback": {
                                                "__dr": "CometGenericCommentDisableNotice.react"
                                            }
                                        },
                                        "replies_connection": {
                                            "edges": [],
                                            "page_info": {
                                                "end_cursor": null,
                                                "has_next_page": false,
                                                "has_previous_page": false,
                                                "start_cursor": null
                                            }
                                        },
                                        "parent_object_ent": {
                                            "__typename": "Comment",
                                            "inline_replies_expander_renderer": null,
                                            "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1Mjc4ODg0MjA1NjY2NjU="
                                        },
                                        "viewer_feedback_reaction_info": null,
                                        "top_reactions": {
                                            "edges": []
                                        },
                                        "reactors": {
                                            "count_reduced": "0",
                                            "count": 0
                                        },
                                        "can_see_top_custom_reactions_on_comment_for_creators": null,
                                        "should_show_top_reactions": false
                                    },
                                    "legacy_fbid": "7527888420566665",
                                    "depth": 0,
                                    "body": {
                                        "text": ",",
                                        "ranges": []
                                    },
                                    "attachments": [],
                                    "is_markdown_enabled": false,
                                    "community_comment_signal_renderer": null,
                                    "comment_menu_tooltip": "Ẩn hoặc báo cáo bình luận này",
                                    "should_show_comment_menu": true,
                                    "author": {
                                        "__typename": "User",
                                        "id": "100081953824049",
                                        "name": "Le Hoang",
                                        "__isActor": "User",
                                        "profile_picture_depth_0": {
                                            "uri": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-1/386452053_303707972370995_1597759332350908646_n.jpg?stp=cp6_dst-jpg_p48x48&_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_ohc=BGHj1eJ8LxEAb5JjmGs&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfCq66yEhWlmYfo_nLFTaZG-08nlidRePdmwUHFBBdx5Hg&oe=6622A178"
                                        },
                                        "profile_picture_depth_1": {
                                            "uri": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-1/386452053_303707972370995_1597759332350908646_n.jpg?stp=cp6_dst-jpg_p40x40&_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_ohc=BGHj1eJ8LxEAb5JjmGs&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfCpDjsHAl4TNi2uiEoD1RjG1rUH-7Wqh0RAeG_vquSYQA&oe=6622A178"
                                        },
                                        "gender": "MALE",
                                        "__isEntity": "User",
                                        "url": "https://www.facebook.com/profile.php?id=100081953824049",
                                        "work_info": null,
                                        "is_verified": false,
                                        "short_name": "Le",
                                        "subscribe_status": "CANNOT_SUBSCRIBE"
                                    },
                                    "is_author_weak_reference": false,
                                    "comment_action_links": [
                                        {
                                            "__typename": "XFBCommentTimeStampActionLink",
                                            "comment": {
                                                "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1Mjc4ODg0MjA1NjY2NjU=",
                                                "created_time": 1713023939,
                                                "url": "https://www.facebook.com/groups/autocsharp/posts/7527887927233381/?comment_id=7527888420566665"
                                            },
                                            "__module_operation_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentTimeStampActionLink_commentActionLink$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentTimeStampActionLink.react"
                                            }
                                        },
                                        {
                                            "__typename": "XFBCommentReactionActionLink",
                                            "comment": {
                                                "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1Mjc4ODg0MjA1NjY2NjU=",
                                                "is_live_video_comment": false,
                                                "feedback": {
                                                    "id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTI3ODg4NDIwNTY2NjY1",
                                                    "viewer_feedback_reaction_info": null,
                                                    "viewer_actor": {
                                                        "__typename": "User",
                                                        "id": "61557504676830"
                                                    },
                                                    "supported_reaction_infos": [
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An_NYk94x95Kypus5FJQ4k1oKEtko7-rUveEhwXytks318UoxoopBczHucoGDTjX4YcuAmIDkUw9SWBKhz7XYoAsQO_zxmWdkseO4YNdrvYmnIdmeAk.kf?ccb=10-5&oh=00_AfC4N59wnCTXy-mqcto-H4aFf0t_dEdWoIbTiBnBpDEN0A&oe=66447038&_nc_sid=7da55a"
                                                            },
                                                            "id": "1635855486666999"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9Tph7xL5aYi3BTTpVl2ow-l1vEv0-qYrBxereq6t6fWgcNnxeyJLsd3DuGnbCLdLFmcvvxn5ivo85wlrIv-EZhT1EucYZ-qoMW0ahYWHGpBBoqSjw.kf?ccb=10-5&oh=00_AfDQ-6lecXmTlchQ-RyfLcosRP1EUCa4krksCPKuOdWCvw&oe=66444D81&_nc_sid=7da55a"
                                                            },
                                                            "id": "1678524932434102"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An-iEpi04A6D-3XVq3wsUCtKdkB4w6IdurXeouCv4FsHYljtXw-fLrmbfC8B8zH5fPrckxLdEzR7V7dfidlNcrNoGsJWxiPDnzyNK-npl_KrJieMlg.kf?ccb=10-5&oh=00_AfAfoDjoOK-htcJ9ZDVYLBbUr_TNAdP_o_8P-R59OVhhig&oe=664475AE&_nc_sid=7da55a"
                                                            },
                                                            "id": "613557422527858"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9yyyXsW_c8BzV1_m0x9WqIPc7IKsshuStlldoUJeshdwMKRkmQmdPEGGwMopV9sH85YDKihkJ8DjNhx1wb2IaUuEOGzE_ji5F9MEXs_50bbA-IXQ.kf?ccb=10-5&oh=00_AfDHdIX2WR5sWRP3EbJwkmXXizlWvkkxyozcLRGko3OFmw&oe=664454A5&_nc_sid=7da55a"
                                                            },
                                                            "id": "115940658764963"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9Ob_EAguyCtqplSNOuikWQ6JjlxIh8vYoEgMXvR0CwneLvNdYwV-1NZgwJfR4aZ4QXhIpQUZxunwGdGubGw20jp-9DikfLbRVh-i4tobncZg9LGpE.kf?ccb=10-5&oh=00_AfBH4f_8b9YpKyqgriHL1hsfvrjLf57CHW4C13NN_Uqp1g&oe=66444171&_nc_sid=7da55a"
                                                            },
                                                            "id": "478547315650144"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9UFu6eXdDopP-SnPAhX-9SngOH_VeoYgHIGK6re6qbARX_PMcNl8Z14QPPFnVzbcfOQwxJxX5q-H5Fy3602EbOrVHhr1m4VSMXypn3fj2NSJongRg.kf?ccb=10-5&oh=00_AfDcHEN-Lj4ZCyxGPwBZoihFPCZSsZd9ZUgr77Gp74G5ag&oe=664467C8&_nc_sid=7da55a"
                                                            },
                                                            "id": "908563459236466"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An919EwtdC17ceBi2men2TIR0UhNUwitUvpE61_Jbs44ggFt3mvLWkKiHP_CSmw72ohKdyEscSIBof6y1FeS57I3kGfh5tg96jndT5mnnEuJlpXuvuUj.kf?ccb=10-5&oh=00_AfD72uYo4bK4mUP0nsihQdCNdL-Eo6WbQt4XeEsX2z2zjw&oe=664465A4&_nc_sid=7da55a"
                                                            },
                                                            "id": "444813342392137"
                                                        }
                                                    ],
                                                    "if_viewer_can_use_creator_custom_reactions": null,
                                                    "associated_video": null,
                                                    "top_reactions": {
                                                        "edges": []
                                                    },
                                                    "unified_reactors": {
                                                        "count": 0
                                                    },
                                                    "reactors": {
                                                        "count": 0,
                                                        "is_empty": true
                                                    },
                                                    "if_viewer_can_render_creator_custom_reactions": null
                                                }
                                            },
                                            "__module_operation_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentReactionActionLink_commentActionLink$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentReactionActionLink.react"
                                            }
                                        },
                                        {
                                            "__typename": "XFBCommentReplyActionLink",
                                            "comment": {
                                                "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1Mjc4ODg0MjA1NjY2NjU=",
                                                "is_live_video_comment": false,
                                                "comment_parent": null,
                                                "is_author_weak_reference": false,
                                                "legacy_fbid": "7527888420566665",
                                                "url": "https://www.facebook.com/groups/autocsharp/posts/7527887927233381/?comment_id=7527888420566665",
                                                "author": {
                                                    "__typename": "User",
                                                    "id": "100081953824049",
                                                    "name": "Le Hoang",
                                                    "url": "https://www.facebook.com/profile.php?id=100081953824049"
                                                },
                                                "feedback": {
                                                    "comment_composer_placeholder": "Viết phản hồi công khai…",
                                                    "id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTI3ODg4NDIwNTY2NjY1"
                                                }
                                            },
                                            "__module_operation_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentReplyActionLink_commentActionLink$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentReplyActionLink.react"
                                            }
                                        },
                                        {
                                            "__typename": "XFBCommentShareActionLink",
                                            "comment": {
                                                "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1Mjc4ODg0MjA1NjY2NjU=",
                                                "url": "https://www.facebook.com/groups/autocsharp/posts/7527887927233381/?comment_id=7527888420566665",
                                                "__isEntity": "Comment",
                                                "__isNode": "Comment"
                                            },
                                            "__module_operation_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentShareActionLinkExperimental_commentActionLink$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentShareActionLinkExperimental.react"
                                            }
                                        }
                                    ],
                                    "preferred_body": {
                                        "__typename": "TextWithEntities",
                                        "delight_ranges": [],
                                        "image_ranges": [],
                                        "inline_style_ranges": [],
                                        "aggregated_ranges": [],
                                        "ranges": [],
                                        "color_ranges": [],
                                        "text": ",",
                                        "translation_type": "ORIGINAL"
                                    },
                                    "body_renderer": {
                                        "__typename": "TextWithEntities",
                                        "delight_ranges": [],
                                        "image_ranges": [],
                                        "inline_style_ranges": [],
                                        "aggregated_ranges": [],
                                        "ranges": [],
                                        "color_ranges": [],
                                        "text": ",",
                                        "__module_operation_CometUFICommentTextBodyRenderer_comment": {
                                            "__dr": "CometUFICommentBodyTextWithEntities_textWithEntities$normalization.graphql"
                                        },
                                        "__module_component_CometUFICommentTextBodyRenderer_comment": {
                                            "__dr": "CometUFICommentBodyTextWithEntities.react"
                                        }
                                    },
                                    "comment_parent": null,
                                    "is_declined_by_group_admin_assistant": false,
                                    "is_gaming_video_comment": false,
                                    "timestamp_in_video": null,
                                    "translatability_for_viewer": {
                                        "source_dialect": ""
                                    },
                                    "written_while_video_was_live": false,
                                    "group_comment_info": {
                                        "group": {
                                            "id": "1777766135578951",
                                            "answer_agent_id": null
                                        },
                                        "is_author_with_member_profile": true,
                                        "__module_operation_CometUFICommentActorLink_comment_groups": {
                                            "__dr": "CometUFIGroupCommentActorLink_groupCommentInfo$normalization.graphql"
                                        },
                                        "__module_component_CometUFICommentActorLink_comment_groups": {
                                            "__dr": "CometUFIGroupCommentActorLink.react"
                                        }
                                    },
                                    "bizweb_comment_info": null,
                                    "has_constituent_badge": false,
                                    "can_viewer_see_subsribe_button": false,
                                    "can_see_constituent_badge_upsell": false,
                                    "legacy_token": "7527887927233381_7527888420566665",
                                    "parent_feedback": {
                                        "id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MQ==",
                                        "share_fbid": "7527887927233381",
                                        "political_figure_data": null,
                                        "owning_profile": {
                                            "__typename": "User",
                                            "name": "Le Hoang",
                                            "id": "100081953824049"
                                        }
                                    },
                                    "question_and_answer_type": null,
                                    "is_author_original_poster": true,
                                    "is_viewer_comment_poster": false,
                                    "is_author_bot": false,
                                    "is_author_non_coworker": false,
                                    "author_user_signals_renderer": {
                                        "__typename": "CometUFICommentActorUserSignalsRenderer",
                                        "user_signals_info": {
                                            "displayed_user_signals": [
                                                {
                                                    "id": "7146222478833280",
                                                    "signal_type_id": "325611522124903",
                                                    "lightModeImage": null,
                                                    "darkModeImage": null,
                                                    "tag_render_info": {
                                                        "comet_detail_view": null,
                                                        "color_variant": "PRIMARY",
                                                        "layout_type": "TEXT_ONLY"
                                                    },
                                                    "title": {
                                                        "text": "Tác giả"
                                                    }
                                                }
                                            ],
                                            "has_more": false,
                                            "overflow_uri": null,
                                            "total_count": 1,
                                            "show_middot": null
                                        },
                                        "__module_operation_CometUFICommentActorLinkBadges_comment": {
                                            "__dr": "CometUFICommentActorUserSignalsRenderer_renderer$normalization.graphql"
                                        },
                                        "__module_component_CometUFICommentActorLinkBadges_comment": {
                                            "__dr": "CometUFICommentActorUserSignalsRenderer.react"
                                        }
                                    },
                                    "author_badge_renderers": [],
                                    "identity_badges_web": [],
                                    "can_show_multiple_identity_badges": false,
                                    "discoverable_identity_badges_web": [],
                                    "user": {
                                        "name": "Le Hoang",
                                        "profile_picture": {
                                            "uri": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-1/386452053_303707972370995_1597759332350908646_n.jpg?stp=cp6_dst-jpg_p80x80&_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_ohc=BGHj1eJ8LxEAb5JjmGs&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfACHQHYIgP20WahdtapSlsLS6CH0RSw09OrVY4PjC5ecg&oe=6622A178"
                                        },
                                        "id": "100081953824049"
                                    },
                                    "parent_post_story": {
                                        "attachments": [],
                                        "id": "UzpfSTEwMDA4MTk1MzgyNDA0OTpWSzo3NTI3ODg3OTI3MjMzMzgx"
                                    },
                                    "work_ama_answer_status": null,
                                    "work_knowledge_inline_annotation_comment_badge_renderer": null,
                                    "business_comment_attributes": [],
                                    "is_live_video_comment": false,
                                    "created_time": 1713023939,
                                    "translation_available_for_viewer": false,
                                    "inline_survey_config": null,
                                    "spam_display_mode": "none",
                                    "attached_story": null,
                                    "helpful_comments_comment_eyebrow_renderer": null,
                                    "comment_direct_parent": null,
                                    "if_viewer_can_see_member_page_tooltip": null,
                                    "is_disabled": false,
                                    "work_answered_event_comment_renderer": null,
                                    "comment_upper_badge_renderer": null,
                                    "elevated_comment_data": null,
                                    "__typename": "Comment"
                                },
                                "cursor": null
                            },
                            {
                                "node": {
                                    "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1Mjc5MTIzMDM4OTc2MTA=",
                                    "feedback": {
                                        "id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTI3OTEyMzAzODk3NjEw",
                                        "expansion_info": {
                                            "expansion_token": "MjoxNzEzMTcxMTYwOgF1XcUxH8hekqpAajOpbsUDQxl_ZejMSZyIVKMPeFZVbmTUWKI1XsGAFJLmrXJqxX4Qvt6Yhs2Irnh2VXyJgaUXHNK8bOt6TdkMevFRBMSMCKFOYmncm7woJIFypYK9RJGR_dpylGYZAsoUo2GjBuojFV_fzn7CTSgMNJU9yOm-IZgwVyeKHioc04X5k6iJBuJWozgZHj12fPVYy0LMtFjKUhYSYPrOry0ggzK1tlnfQ9HcFu3I7FuBqWxj6GN-Q7oDXmBQ9REmT3z_rSyw1xzgiN_wNLODqbg_q0eQDgth79qC9y6JjfHTmjvHgJyt64kLmhoChHMF9UYBzdqSWCdJ1AT32Z__SwmH0L0OWtmue6oFTUXzsKr30LgHiGs2jF8R6hy_TZ586mjhBRECzti21F_FQsGzDg-XE4-bZjVuW60_klwk7w1Lc5LWJzAjEIIUul46ZcNiLHoX_Hs3PEbeRjeYZOSMldkiOc7_T3Fpj1Z5f737mCQdvgAvBZOwzBsDZfWLIMkOpU7psIw",
                                            "should_show_reply_count": true
                                        },
                                        "replies_fields": {
                                            "filtering_footer_string": "",
                                            "count": 0,
                                            "total_count": 0
                                        },
                                        "viewer_actor": {
                                            "__typename": "User",
                                            "id": "61557504676830",
                                            "__isActor": "User",
                                            "name": "Lý Mai",
                                            "profile_picture_depth_0": {
                                                "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t1.30497-1/143086968_2856368904622192_1959732218791162458_n.png?stp=cp0_dst-png_p48x48&_nc_cat=1&ccb=1-7&_nc_sid=5f2048&_nc_ohc=kNSgHQLZ6doAb7eTDui&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDEoIPJUkx_mGovM_J3326vyBlc9auyJo-PJ_EBTtGgRg&oe=66445C78"
                                            },
                                            "profile_picture_depth_1": {
                                                "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t1.30497-1/143086968_2856368904622192_1959732218791162458_n.png?stp=cp0_dst-png_p40x40&_nc_cat=1&ccb=1-7&_nc_sid=5f2048&_nc_ohc=kNSgHQLZ6doAb7eTDui&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDqYKF91_-oKl07Nqn6ibjv0dysE8eyQkwL7oXXxsmLDA&oe=66445C78"
                                            },
                                            "gender": "MALE"
                                        },
                                        "url": "https://www.facebook.com/groups/autocsharp/posts/7527887927233381/?comment_id=7527912303897610",
                                        "__typename": "Feedback",
                                        "plugins": [
                                            {
                                                "__typename": "CommentComposerGroupMentionsPlugin",
                                                "group_id": "1777766135578951",
                                                "post_id": "7527912303897610",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerGroupMentionsPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerGroupMentionsPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerAvatarPlugin",
                                                "has_avatar": false,
                                                "feedback_id": "7527912303897610",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerAvatarPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerAvatarPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerHashtagPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerHashtagPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerHashtagPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerEmojiPlugin",
                                                "emoji_size": 16,
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerEmojiPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerEmojiPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerMediaUploadPlugin",
                                                "viewer_actor": {
                                                    "__typename": "User",
                                                    "id": "61557504676830"
                                                },
                                                "should_condense_video_preview": true,
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerMediaUploadPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerMediaUploadPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerGIFPlugin",
                                                "feedback_id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTI3OTEyMzAzODk3NjEw",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerGIFPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerGIFPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CometComposerCometizedStickersPlugin",
                                                "feedback_id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTI3OTEyMzAzODk3NjEw",
                                                "owning_profile_id": "100081953824049",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerStickersPlugin_next_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerStickersPlugin.next"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerEmoticonPlugin",
                                                "emoji_size": 16,
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerEmoticonPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerEmoticonPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerPrefillMentionPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerPrefillMentionPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerPrefillMentionPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerAssociateReplyWithParentPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerAssociateReplyWithParentPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerAssociateReplyWithParentPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerSetReplyClickedPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerSetReplyClickedPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerSetReplyClickedPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerStateSnapshotPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerStateSnapshotPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerStateSnapshotPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerLiveTypingBroadcastPlugin",
                                                "feedback_id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTI3OTEyMzAzODk3NjEw",
                                                "viewer_actor": {
                                                    "__typename": "User",
                                                    "id": "61557504676830"
                                                },
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerLiveTypingBroadcastPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerLiveTypingBroadcastPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerCommentCharacterLimitPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerCommentCharacterLimitPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerCommentCharacterLimitPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerWriteToComposerPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerWriteToComposerPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerWriteToComposerPlugin"
                                                }
                                            }
                                        ],
                                        "comment_composer_placeholder": "Viết phản hồi công khai…",
                                        "can_viewer_comment": true,
                                        "constituent_badge_banner_renderer": null,
                                        "have_comments_been_disabled": false,
                                        "are_live_video_comments_disabled": false,
                                        "is_viewer_muted": false,
                                        "total_comment_count": 0,
                                        "comments_disabled_notice_renderer": {
                                            "__typename": "GeneralCommentDisableNotice",
                                            "notice_message": {
                                                "delight_ranges": [],
                                                "image_ranges": [],
                                                "inline_style_ranges": [],
                                                "aggregated_ranges": [],
                                                "ranges": [],
                                                "color_ranges": [],
                                                "text": "Bình luận đã bị tắt cho bài viết này."
                                            },
                                            "__module_operation_CometUFICommentDisabledNotice_feedback": {
                                                "__dr": "CometGenericCommentDisableNotice_commentDisableNotice$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentDisabledNotice_feedback": {
                                                "__dr": "CometGenericCommentDisableNotice.react"
                                            }
                                        },
                                        "replies_connection": {
                                            "edges": [],
                                            "page_info": {
                                                "end_cursor": null,
                                                "has_next_page": false,
                                                "has_previous_page": false,
                                                "start_cursor": null
                                            }
                                        },
                                        "parent_object_ent": {
                                            "__typename": "Comment",
                                            "inline_replies_expander_renderer": null,
                                            "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1Mjc5MTIzMDM4OTc2MTA="
                                        },
                                        "viewer_feedback_reaction_info": null,
                                        "top_reactions": {
                                            "edges": []
                                        },
                                        "reactors": {
                                            "count_reduced": "0",
                                            "count": 0
                                        },
                                        "can_see_top_custom_reactions_on_comment_for_creators": null,
                                        "should_show_top_reactions": false
                                    },
                                    "legacy_fbid": "7527912303897610",
                                    "depth": 0,
                                    "body": {
                                        "text": ",",
                                        "ranges": []
                                    },
                                    "attachments": [],
                                    "is_markdown_enabled": false,
                                    "community_comment_signal_renderer": null,
                                    "comment_menu_tooltip": "Ẩn hoặc báo cáo bình luận này",
                                    "should_show_comment_menu": true,
                                    "author": {
                                        "__typename": "User",
                                        "id": "100081953824049",
                                        "name": "Le Hoang",
                                        "__isActor": "User",
                                        "profile_picture_depth_0": {
                                            "uri": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-1/386452053_303707972370995_1597759332350908646_n.jpg?stp=cp6_dst-jpg_p48x48&_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_ohc=BGHj1eJ8LxEAb5JjmGs&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfCq66yEhWlmYfo_nLFTaZG-08nlidRePdmwUHFBBdx5Hg&oe=6622A178"
                                        },
                                        "profile_picture_depth_1": {
                                            "uri": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-1/386452053_303707972370995_1597759332350908646_n.jpg?stp=cp6_dst-jpg_p40x40&_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_ohc=BGHj1eJ8LxEAb5JjmGs&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfCpDjsHAl4TNi2uiEoD1RjG1rUH-7Wqh0RAeG_vquSYQA&oe=6622A178"
                                        },
                                        "gender": "MALE",
                                        "__isEntity": "User",
                                        "url": "https://www.facebook.com/profile.php?id=100081953824049",
                                        "work_info": null,
                                        "is_verified": false,
                                        "short_name": "Le",
                                        "subscribe_status": "CANNOT_SUBSCRIBE"
                                    },
                                    "is_author_weak_reference": false,
                                    "comment_action_links": [
                                        {
                                            "__typename": "XFBCommentTimeStampActionLink",
                                            "comment": {
                                                "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1Mjc5MTIzMDM4OTc2MTA=",
                                                "created_time": 1713024374,
                                                "url": "https://www.facebook.com/groups/autocsharp/posts/7527887927233381/?comment_id=7527912303897610"
                                            },
                                            "__module_operation_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentTimeStampActionLink_commentActionLink$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentTimeStampActionLink.react"
                                            }
                                        },
                                        {
                                            "__typename": "XFBCommentReactionActionLink",
                                            "comment": {
                                                "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1Mjc5MTIzMDM4OTc2MTA=",
                                                "is_live_video_comment": false,
                                                "feedback": {
                                                    "id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTI3OTEyMzAzODk3NjEw",
                                                    "viewer_feedback_reaction_info": null,
                                                    "viewer_actor": {
                                                        "__typename": "User",
                                                        "id": "61557504676830"
                                                    },
                                                    "supported_reaction_infos": [
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An_NYk94x95Kypus5FJQ4k1oKEtko7-rUveEhwXytks318UoxoopBczHucoGDTjX4YcuAmIDkUw9SWBKhz7XYoAsQO_zxmWdkseO4YNdrvYmnIdmeAk.kf?ccb=10-5&oh=00_AfC4N59wnCTXy-mqcto-H4aFf0t_dEdWoIbTiBnBpDEN0A&oe=66447038&_nc_sid=7da55a"
                                                            },
                                                            "id": "1635855486666999"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9Tph7xL5aYi3BTTpVl2ow-l1vEv0-qYrBxereq6t6fWgcNnxeyJLsd3DuGnbCLdLFmcvvxn5ivo85wlrIv-EZhT1EucYZ-qoMW0ahYWHGpBBoqSjw.kf?ccb=10-5&oh=00_AfDQ-6lecXmTlchQ-RyfLcosRP1EUCa4krksCPKuOdWCvw&oe=66444D81&_nc_sid=7da55a"
                                                            },
                                                            "id": "1678524932434102"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An-iEpi04A6D-3XVq3wsUCtKdkB4w6IdurXeouCv4FsHYljtXw-fLrmbfC8B8zH5fPrckxLdEzR7V7dfidlNcrNoGsJWxiPDnzyNK-npl_KrJieMlg.kf?ccb=10-5&oh=00_AfAfoDjoOK-htcJ9ZDVYLBbUr_TNAdP_o_8P-R59OVhhig&oe=664475AE&_nc_sid=7da55a"
                                                            },
                                                            "id": "613557422527858"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9yyyXsW_c8BzV1_m0x9WqIPc7IKsshuStlldoUJeshdwMKRkmQmdPEGGwMopV9sH85YDKihkJ8DjNhx1wb2IaUuEOGzE_ji5F9MEXs_50bbA-IXQ.kf?ccb=10-5&oh=00_AfDHdIX2WR5sWRP3EbJwkmXXizlWvkkxyozcLRGko3OFmw&oe=664454A5&_nc_sid=7da55a"
                                                            },
                                                            "id": "115940658764963"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9Ob_EAguyCtqplSNOuikWQ6JjlxIh8vYoEgMXvR0CwneLvNdYwV-1NZgwJfR4aZ4QXhIpQUZxunwGdGubGw20jp-9DikfLbRVh-i4tobncZg9LGpE.kf?ccb=10-5&oh=00_AfBH4f_8b9YpKyqgriHL1hsfvrjLf57CHW4C13NN_Uqp1g&oe=66444171&_nc_sid=7da55a"
                                                            },
                                                            "id": "478547315650144"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9UFu6eXdDopP-SnPAhX-9SngOH_VeoYgHIGK6re6qbARX_PMcNl8Z14QPPFnVzbcfOQwxJxX5q-H5Fy3602EbOrVHhr1m4VSMXypn3fj2NSJongRg.kf?ccb=10-5&oh=00_AfDcHEN-Lj4ZCyxGPwBZoihFPCZSsZd9ZUgr77Gp74G5ag&oe=664467C8&_nc_sid=7da55a"
                                                            },
                                                            "id": "908563459236466"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An919EwtdC17ceBi2men2TIR0UhNUwitUvpE61_Jbs44ggFt3mvLWkKiHP_CSmw72ohKdyEscSIBof6y1FeS57I3kGfh5tg96jndT5mnnEuJlpXuvuUj.kf?ccb=10-5&oh=00_AfD72uYo4bK4mUP0nsihQdCNdL-Eo6WbQt4XeEsX2z2zjw&oe=664465A4&_nc_sid=7da55a"
                                                            },
                                                            "id": "444813342392137"
                                                        }
                                                    ],
                                                    "if_viewer_can_use_creator_custom_reactions": null,
                                                    "associated_video": null,
                                                    "top_reactions": {
                                                        "edges": []
                                                    },
                                                    "unified_reactors": {
                                                        "count": 0
                                                    },
                                                    "reactors": {
                                                        "count": 0,
                                                        "is_empty": true
                                                    },
                                                    "if_viewer_can_render_creator_custom_reactions": null
                                                }
                                            },
                                            "__module_operation_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentReactionActionLink_commentActionLink$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentReactionActionLink.react"
                                            }
                                        },
                                        {
                                            "__typename": "XFBCommentReplyActionLink",
                                            "comment": {
                                                "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1Mjc5MTIzMDM4OTc2MTA=",
                                                "is_live_video_comment": false,
                                                "comment_parent": null,
                                                "is_author_weak_reference": false,
                                                "legacy_fbid": "7527912303897610",
                                                "url": "https://www.facebook.com/groups/autocsharp/posts/7527887927233381/?comment_id=7527912303897610",
                                                "author": {
                                                    "__typename": "User",
                                                    "id": "100081953824049",
                                                    "name": "Le Hoang",
                                                    "url": "https://www.facebook.com/profile.php?id=100081953824049"
                                                },
                                                "feedback": {
                                                    "comment_composer_placeholder": "Viết phản hồi công khai…",
                                                    "id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTI3OTEyMzAzODk3NjEw"
                                                }
                                            },
                                            "__module_operation_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentReplyActionLink_commentActionLink$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentReplyActionLink.react"
                                            }
                                        },
                                        {
                                            "__typename": "XFBCommentShareActionLink",
                                            "comment": {
                                                "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1Mjc5MTIzMDM4OTc2MTA=",
                                                "url": "https://www.facebook.com/groups/autocsharp/posts/7527887927233381/?comment_id=7527912303897610",
                                                "__isEntity": "Comment",
                                                "__isNode": "Comment"
                                            },
                                            "__module_operation_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentShareActionLinkExperimental_commentActionLink$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentShareActionLinkExperimental.react"
                                            }
                                        }
                                    ],
                                    "preferred_body": {
                                        "__typename": "TextWithEntities",
                                        "delight_ranges": [],
                                        "image_ranges": [],
                                        "inline_style_ranges": [],
                                        "aggregated_ranges": [],
                                        "ranges": [],
                                        "color_ranges": [],
                                        "text": ",",
                                        "translation_type": "ORIGINAL"
                                    },
                                    "body_renderer": {
                                        "__typename": "TextWithEntities",
                                        "delight_ranges": [],
                                        "image_ranges": [],
                                        "inline_style_ranges": [],
                                        "aggregated_ranges": [],
                                        "ranges": [],
                                        "color_ranges": [],
                                        "text": ",",
                                        "__module_operation_CometUFICommentTextBodyRenderer_comment": {
                                            "__dr": "CometUFICommentBodyTextWithEntities_textWithEntities$normalization.graphql"
                                        },
                                        "__module_component_CometUFICommentTextBodyRenderer_comment": {
                                            "__dr": "CometUFICommentBodyTextWithEntities.react"
                                        }
                                    },
                                    "comment_parent": null,
                                    "is_declined_by_group_admin_assistant": false,
                                    "is_gaming_video_comment": false,
                                    "timestamp_in_video": null,
                                    "translatability_for_viewer": {
                                        "source_dialect": ""
                                    },
                                    "written_while_video_was_live": false,
                                    "group_comment_info": {
                                        "group": {
                                            "id": "1777766135578951",
                                            "answer_agent_id": null
                                        },
                                        "is_author_with_member_profile": true,
                                        "__module_operation_CometUFICommentActorLink_comment_groups": {
                                            "__dr": "CometUFIGroupCommentActorLink_groupCommentInfo$normalization.graphql"
                                        },
                                        "__module_component_CometUFICommentActorLink_comment_groups": {
                                            "__dr": "CometUFIGroupCommentActorLink.react"
                                        }
                                    },
                                    "bizweb_comment_info": null,
                                    "has_constituent_badge": false,
                                    "can_viewer_see_subsribe_button": false,
                                    "can_see_constituent_badge_upsell": false,
                                    "legacy_token": "7527887927233381_7527912303897610",
                                    "parent_feedback": {
                                        "id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MQ==",
                                        "share_fbid": "7527887927233381",
                                        "political_figure_data": null,
                                        "owning_profile": {
                                            "__typename": "User",
                                            "name": "Le Hoang",
                                            "id": "100081953824049"
                                        }
                                    },
                                    "question_and_answer_type": null,
                                    "is_author_original_poster": true,
                                    "is_viewer_comment_poster": false,
                                    "is_author_bot": false,
                                    "is_author_non_coworker": false,
                                    "author_user_signals_renderer": {
                                        "__typename": "CometUFICommentActorUserSignalsRenderer",
                                        "user_signals_info": {
                                            "displayed_user_signals": [
                                                {
                                                    "id": "6761944290573684",
                                                    "signal_type_id": "325611522124903",
                                                    "lightModeImage": null,
                                                    "darkModeImage": null,
                                                    "tag_render_info": {
                                                        "comet_detail_view": null,
                                                        "color_variant": "PRIMARY",
                                                        "layout_type": "TEXT_ONLY"
                                                    },
                                                    "title": {
                                                        "text": "Tác giả"
                                                    }
                                                }
                                            ],
                                            "has_more": false,
                                            "overflow_uri": null,
                                            "total_count": 1,
                                            "show_middot": null
                                        },
                                        "__module_operation_CometUFICommentActorLinkBadges_comment": {
                                            "__dr": "CometUFICommentActorUserSignalsRenderer_renderer$normalization.graphql"
                                        },
                                        "__module_component_CometUFICommentActorLinkBadges_comment": {
                                            "__dr": "CometUFICommentActorUserSignalsRenderer.react"
                                        }
                                    },
                                    "author_badge_renderers": [],
                                    "identity_badges_web": [],
                                    "can_show_multiple_identity_badges": false,
                                    "discoverable_identity_badges_web": [],
                                    "user": {
                                        "name": "Le Hoang",
                                        "profile_picture": {
                                            "uri": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-1/386452053_303707972370995_1597759332350908646_n.jpg?stp=cp6_dst-jpg_p80x80&_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_ohc=BGHj1eJ8LxEAb5JjmGs&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfACHQHYIgP20WahdtapSlsLS6CH0RSw09OrVY4PjC5ecg&oe=6622A178"
                                        },
                                        "id": "100081953824049"
                                    },
                                    "parent_post_story": {
                                        "attachments": [],
                                        "id": "UzpfSTEwMDA4MTk1MzgyNDA0OTpWSzo3NTI3ODg3OTI3MjMzMzgx"
                                    },
                                    "work_ama_answer_status": null,
                                    "work_knowledge_inline_annotation_comment_badge_renderer": null,
                                    "business_comment_attributes": [],
                                    "is_live_video_comment": false,
                                    "created_time": 1713024374,
                                    "translation_available_for_viewer": false,
                                    "inline_survey_config": null,
                                    "spam_display_mode": "none",
                                    "attached_story": null,
                                    "helpful_comments_comment_eyebrow_renderer": null,
                                    "comment_direct_parent": null,
                                    "if_viewer_can_see_member_page_tooltip": null,
                                    "is_disabled": false,
                                    "work_answered_event_comment_renderer": null,
                                    "comment_upper_badge_renderer": null,
                                    "elevated_comment_data": null,
                                    "__typename": "Comment"
                                },
                                "cursor": null
                            },
                            {
                                "node": {
                                    "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1Mjc5MzUxNTA1NjE5OTI=",
                                    "feedback": {
                                        "id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTI3OTM1MTUwNTYxOTky",
                                        "expansion_info": {
                                            "expansion_token": "MjoxNzEzMTcxMTYwOgF1kZvB0PhAIDMHuMa4mDewX9ic2a3Ll3C0QWLEjNq_l86TW6RpMnpzpJoi3DEZHvmI0T2TRa-AgK9q8WWdPHrdxwJxi46vgGAKNpJbqw5wVQT51VdNHwvsD9gLm9PV0gJooVaiwt7y5nY9QQk7MzC5wRwbAD0dwzcI6S530wlplRS6O3oTn5GBcfhQQxSsBUQhHLYVkBFs66RCtRNj0rkVZcDlCXpd72tqsXI67QzYQJOnFypaZXKIUZfi119NJ2y5QcLMGS9f6J1A-5oiH4tTYXw_LmNoHq7Ud9DAfIypT6FzRkAixo6IVnPkrq5qQ9IZKXbMMCC6F3nCfnk-tChweR6VUkIGCdF2bZydGRLvA7wunJNmagJpGXTwHPYe7JsTVEpwYbYXfq6KdAD3yauFrxdRdqKlyJWiCzK_eIa88bSdLLV0nz9ooxzne_y0h_c6npN2qWBYSjtmKG-MU_9NhZ8wALgArmi-R3qAp2Tz_U0urXJ2vmvolMe4Wa_J_Ir9jA3BL0Hnni3kmrw",
                                            "should_show_reply_count": true
                                        },
                                        "replies_fields": {
                                            "filtering_footer_string": "",
                                            "count": 0,
                                            "total_count": 0
                                        },
                                        "viewer_actor": {
                                            "__typename": "User",
                                            "id": "61557504676830",
                                            "__isActor": "User",
                                            "name": "Lý Mai",
                                            "profile_picture_depth_0": {
                                                "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t1.30497-1/143086968_2856368904622192_1959732218791162458_n.png?stp=cp0_dst-png_p48x48&_nc_cat=1&ccb=1-7&_nc_sid=5f2048&_nc_ohc=kNSgHQLZ6doAb7eTDui&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDEoIPJUkx_mGovM_J3326vyBlc9auyJo-PJ_EBTtGgRg&oe=66445C78"
                                            },
                                            "profile_picture_depth_1": {
                                                "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t1.30497-1/143086968_2856368904622192_1959732218791162458_n.png?stp=cp0_dst-png_p40x40&_nc_cat=1&ccb=1-7&_nc_sid=5f2048&_nc_ohc=kNSgHQLZ6doAb7eTDui&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDqYKF91_-oKl07Nqn6ibjv0dysE8eyQkwL7oXXxsmLDA&oe=66445C78"
                                            },
                                            "gender": "MALE"
                                        },
                                        "url": "https://www.facebook.com/groups/autocsharp/posts/7527887927233381/?comment_id=7527935150561992",
                                        "__typename": "Feedback",
                                        "plugins": [
                                            {
                                                "__typename": "CommentComposerGroupMentionsPlugin",
                                                "group_id": "1777766135578951",
                                                "post_id": "7527935150561992",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerGroupMentionsPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerGroupMentionsPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerAvatarPlugin",
                                                "has_avatar": false,
                                                "feedback_id": "7527935150561992",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerAvatarPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerAvatarPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerHashtagPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerHashtagPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerHashtagPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerEmojiPlugin",
                                                "emoji_size": 16,
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerEmojiPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerEmojiPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerMediaUploadPlugin",
                                                "viewer_actor": {
                                                    "__typename": "User",
                                                    "id": "61557504676830"
                                                },
                                                "should_condense_video_preview": true,
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerMediaUploadPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerMediaUploadPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerGIFPlugin",
                                                "feedback_id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTI3OTM1MTUwNTYxOTky",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerGIFPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerGIFPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CometComposerCometizedStickersPlugin",
                                                "feedback_id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTI3OTM1MTUwNTYxOTky",
                                                "owning_profile_id": "100081953824049",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerStickersPlugin_next_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerStickersPlugin.next"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerEmoticonPlugin",
                                                "emoji_size": 16,
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerEmoticonPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerEmoticonPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerPrefillMentionPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerPrefillMentionPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerPrefillMentionPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerAssociateReplyWithParentPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerAssociateReplyWithParentPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerAssociateReplyWithParentPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerSetReplyClickedPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerSetReplyClickedPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerSetReplyClickedPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerStateSnapshotPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerStateSnapshotPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerStateSnapshotPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerLiveTypingBroadcastPlugin",
                                                "feedback_id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTI3OTM1MTUwNTYxOTky",
                                                "viewer_actor": {
                                                    "__typename": "User",
                                                    "id": "61557504676830"
                                                },
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerLiveTypingBroadcastPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerLiveTypingBroadcastPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerCommentCharacterLimitPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerCommentCharacterLimitPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerCommentCharacterLimitPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerWriteToComposerPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerWriteToComposerPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerWriteToComposerPlugin"
                                                }
                                            }
                                        ],
                                        "comment_composer_placeholder": "Viết phản hồi công khai…",
                                        "can_viewer_comment": true,
                                        "constituent_badge_banner_renderer": null,
                                        "have_comments_been_disabled": false,
                                        "are_live_video_comments_disabled": false,
                                        "is_viewer_muted": false,
                                        "total_comment_count": 0,
                                        "comments_disabled_notice_renderer": {
                                            "__typename": "GeneralCommentDisableNotice",
                                            "notice_message": {
                                                "delight_ranges": [],
                                                "image_ranges": [],
                                                "inline_style_ranges": [],
                                                "aggregated_ranges": [],
                                                "ranges": [],
                                                "color_ranges": [],
                                                "text": "Bình luận đã bị tắt cho bài viết này."
                                            },
                                            "__module_operation_CometUFICommentDisabledNotice_feedback": {
                                                "__dr": "CometGenericCommentDisableNotice_commentDisableNotice$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentDisabledNotice_feedback": {
                                                "__dr": "CometGenericCommentDisableNotice.react"
                                            }
                                        },
                                        "replies_connection": {
                                            "edges": [],
                                            "page_info": {
                                                "end_cursor": null,
                                                "has_next_page": false,
                                                "has_previous_page": false,
                                                "start_cursor": null
                                            }
                                        },
                                        "parent_object_ent": {
                                            "__typename": "Comment",
                                            "inline_replies_expander_renderer": null,
                                            "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1Mjc5MzUxNTA1NjE5OTI="
                                        },
                                        "viewer_feedback_reaction_info": null,
                                        "top_reactions": {
                                            "edges": []
                                        },
                                        "reactors": {
                                            "count_reduced": "0",
                                            "count": 0
                                        },
                                        "can_see_top_custom_reactions_on_comment_for_creators": null,
                                        "should_show_top_reactions": false
                                    },
                                    "legacy_fbid": "7527935150561992",
                                    "depth": 0,
                                    "body": {
                                        "text": "Hi",
                                        "ranges": []
                                    },
                                    "attachments": [],
                                    "is_markdown_enabled": false,
                                    "community_comment_signal_renderer": null,
                                    "comment_menu_tooltip": "Ẩn hoặc báo cáo bình luận này",
                                    "should_show_comment_menu": true,
                                    "author": {
                                        "__typename": "User",
                                        "id": "100081953824049",
                                        "name": "Le Hoang",
                                        "__isActor": "User",
                                        "profile_picture_depth_0": {
                                            "uri": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-1/386452053_303707972370995_1597759332350908646_n.jpg?stp=cp6_dst-jpg_p48x48&_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_ohc=BGHj1eJ8LxEAb5JjmGs&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfCq66yEhWlmYfo_nLFTaZG-08nlidRePdmwUHFBBdx5Hg&oe=6622A178"
                                        },
                                        "profile_picture_depth_1": {
                                            "uri": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-1/386452053_303707972370995_1597759332350908646_n.jpg?stp=cp6_dst-jpg_p40x40&_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_ohc=BGHj1eJ8LxEAb5JjmGs&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfCpDjsHAl4TNi2uiEoD1RjG1rUH-7Wqh0RAeG_vquSYQA&oe=6622A178"
                                        },
                                        "gender": "MALE",
                                        "__isEntity": "User",
                                        "url": "https://www.facebook.com/profile.php?id=100081953824049",
                                        "work_info": null,
                                        "is_verified": false,
                                        "short_name": "Le",
                                        "subscribe_status": "CANNOT_SUBSCRIBE"
                                    },
                                    "is_author_weak_reference": false,
                                    "comment_action_links": [
                                        {
                                            "__typename": "XFBCommentTimeStampActionLink",
                                            "comment": {
                                                "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1Mjc5MzUxNTA1NjE5OTI=",
                                                "created_time": 1713024780,
                                                "url": "https://www.facebook.com/groups/autocsharp/posts/7527887927233381/?comment_id=7527935150561992"
                                            },
                                            "__module_operation_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentTimeStampActionLink_commentActionLink$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentTimeStampActionLink.react"
                                            }
                                        },
                                        {
                                            "__typename": "XFBCommentReactionActionLink",
                                            "comment": {
                                                "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1Mjc5MzUxNTA1NjE5OTI=",
                                                "is_live_video_comment": false,
                                                "feedback": {
                                                    "id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTI3OTM1MTUwNTYxOTky",
                                                    "viewer_feedback_reaction_info": null,
                                                    "viewer_actor": {
                                                        "__typename": "User",
                                                        "id": "61557504676830"
                                                    },
                                                    "supported_reaction_infos": [
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An_NYk94x95Kypus5FJQ4k1oKEtko7-rUveEhwXytks318UoxoopBczHucoGDTjX4YcuAmIDkUw9SWBKhz7XYoAsQO_zxmWdkseO4YNdrvYmnIdmeAk.kf?ccb=10-5&oh=00_AfC4N59wnCTXy-mqcto-H4aFf0t_dEdWoIbTiBnBpDEN0A&oe=66447038&_nc_sid=7da55a"
                                                            },
                                                            "id": "1635855486666999"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9Tph7xL5aYi3BTTpVl2ow-l1vEv0-qYrBxereq6t6fWgcNnxeyJLsd3DuGnbCLdLFmcvvxn5ivo85wlrIv-EZhT1EucYZ-qoMW0ahYWHGpBBoqSjw.kf?ccb=10-5&oh=00_AfDQ-6lecXmTlchQ-RyfLcosRP1EUCa4krksCPKuOdWCvw&oe=66444D81&_nc_sid=7da55a"
                                                            },
                                                            "id": "1678524932434102"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An-iEpi04A6D-3XVq3wsUCtKdkB4w6IdurXeouCv4FsHYljtXw-fLrmbfC8B8zH5fPrckxLdEzR7V7dfidlNcrNoGsJWxiPDnzyNK-npl_KrJieMlg.kf?ccb=10-5&oh=00_AfAfoDjoOK-htcJ9ZDVYLBbUr_TNAdP_o_8P-R59OVhhig&oe=664475AE&_nc_sid=7da55a"
                                                            },
                                                            "id": "613557422527858"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9yyyXsW_c8BzV1_m0x9WqIPc7IKsshuStlldoUJeshdwMKRkmQmdPEGGwMopV9sH85YDKihkJ8DjNhx1wb2IaUuEOGzE_ji5F9MEXs_50bbA-IXQ.kf?ccb=10-5&oh=00_AfDHdIX2WR5sWRP3EbJwkmXXizlWvkkxyozcLRGko3OFmw&oe=664454A5&_nc_sid=7da55a"
                                                            },
                                                            "id": "115940658764963"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9Ob_EAguyCtqplSNOuikWQ6JjlxIh8vYoEgMXvR0CwneLvNdYwV-1NZgwJfR4aZ4QXhIpQUZxunwGdGubGw20jp-9DikfLbRVh-i4tobncZg9LGpE.kf?ccb=10-5&oh=00_AfBH4f_8b9YpKyqgriHL1hsfvrjLf57CHW4C13NN_Uqp1g&oe=66444171&_nc_sid=7da55a"
                                                            },
                                                            "id": "478547315650144"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9UFu6eXdDopP-SnPAhX-9SngOH_VeoYgHIGK6re6qbARX_PMcNl8Z14QPPFnVzbcfOQwxJxX5q-H5Fy3602EbOrVHhr1m4VSMXypn3fj2NSJongRg.kf?ccb=10-5&oh=00_AfDcHEN-Lj4ZCyxGPwBZoihFPCZSsZd9ZUgr77Gp74G5ag&oe=664467C8&_nc_sid=7da55a"
                                                            },
                                                            "id": "908563459236466"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An919EwtdC17ceBi2men2TIR0UhNUwitUvpE61_Jbs44ggFt3mvLWkKiHP_CSmw72ohKdyEscSIBof6y1FeS57I3kGfh5tg96jndT5mnnEuJlpXuvuUj.kf?ccb=10-5&oh=00_AfD72uYo4bK4mUP0nsihQdCNdL-Eo6WbQt4XeEsX2z2zjw&oe=664465A4&_nc_sid=7da55a"
                                                            },
                                                            "id": "444813342392137"
                                                        }
                                                    ],
                                                    "if_viewer_can_use_creator_custom_reactions": null,
                                                    "associated_video": null,
                                                    "top_reactions": {
                                                        "edges": []
                                                    },
                                                    "unified_reactors": {
                                                        "count": 0
                                                    },
                                                    "reactors": {
                                                        "count": 0,
                                                        "is_empty": true
                                                    },
                                                    "if_viewer_can_render_creator_custom_reactions": null
                                                }
                                            },
                                            "__module_operation_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentReactionActionLink_commentActionLink$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentReactionActionLink.react"
                                            }
                                        },
                                        {
                                            "__typename": "XFBCommentReplyActionLink",
                                            "comment": {
                                                "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1Mjc5MzUxNTA1NjE5OTI=",
                                                "is_live_video_comment": false,
                                                "comment_parent": null,
                                                "is_author_weak_reference": false,
                                                "legacy_fbid": "7527935150561992",
                                                "url": "https://www.facebook.com/groups/autocsharp/posts/7527887927233381/?comment_id=7527935150561992",
                                                "author": {
                                                    "__typename": "User",
                                                    "id": "100081953824049",
                                                    "name": "Le Hoang",
                                                    "url": "https://www.facebook.com/profile.php?id=100081953824049"
                                                },
                                                "feedback": {
                                                    "comment_composer_placeholder": "Viết phản hồi công khai…",
                                                    "id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTI3OTM1MTUwNTYxOTky"
                                                }
                                            },
                                            "__module_operation_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentReplyActionLink_commentActionLink$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentReplyActionLink.react"
                                            }
                                        },
                                        {
                                            "__typename": "XFBCommentShareActionLink",
                                            "comment": {
                                                "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1Mjc5MzUxNTA1NjE5OTI=",
                                                "url": "https://www.facebook.com/groups/autocsharp/posts/7527887927233381/?comment_id=7527935150561992",
                                                "__isEntity": "Comment",
                                                "__isNode": "Comment"
                                            },
                                            "__module_operation_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentShareActionLinkExperimental_commentActionLink$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentShareActionLinkExperimental.react"
                                            }
                                        }
                                    ],
                                    "preferred_body": {
                                        "__typename": "TextWithEntities",
                                        "delight_ranges": [],
                                        "image_ranges": [],
                                        "inline_style_ranges": [],
                                        "aggregated_ranges": [],
                                        "ranges": [],
                                        "color_ranges": [],
                                        "text": "Hi",
                                        "translation_type": "ORIGINAL"
                                    },
                                    "body_renderer": {
                                        "__typename": "TextWithEntities",
                                        "delight_ranges": [],
                                        "image_ranges": [],
                                        "inline_style_ranges": [],
                                        "aggregated_ranges": [],
                                        "ranges": [],
                                        "color_ranges": [],
                                        "text": "Hi",
                                        "__module_operation_CometUFICommentTextBodyRenderer_comment": {
                                            "__dr": "CometUFICommentBodyTextWithEntities_textWithEntities$normalization.graphql"
                                        },
                                        "__module_component_CometUFICommentTextBodyRenderer_comment": {
                                            "__dr": "CometUFICommentBodyTextWithEntities.react"
                                        }
                                    },
                                    "comment_parent": null,
                                    "is_declined_by_group_admin_assistant": false,
                                    "is_gaming_video_comment": false,
                                    "timestamp_in_video": null,
                                    "translatability_for_viewer": {
                                        "source_dialect": "en_XX"
                                    },
                                    "written_while_video_was_live": false,
                                    "group_comment_info": {
                                        "group": {
                                            "id": "1777766135578951",
                                            "answer_agent_id": null
                                        },
                                        "is_author_with_member_profile": true,
                                        "__module_operation_CometUFICommentActorLink_comment_groups": {
                                            "__dr": "CometUFIGroupCommentActorLink_groupCommentInfo$normalization.graphql"
                                        },
                                        "__module_component_CometUFICommentActorLink_comment_groups": {
                                            "__dr": "CometUFIGroupCommentActorLink.react"
                                        }
                                    },
                                    "bizweb_comment_info": null,
                                    "has_constituent_badge": false,
                                    "can_viewer_see_subsribe_button": false,
                                    "can_see_constituent_badge_upsell": false,
                                    "legacy_token": "7527887927233381_7527935150561992",
                                    "parent_feedback": {
                                        "id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MQ==",
                                        "share_fbid": "7527887927233381",
                                        "political_figure_data": null,
                                        "owning_profile": {
                                            "__typename": "User",
                                            "name": "Le Hoang",
                                            "id": "100081953824049"
                                        }
                                    },
                                    "question_and_answer_type": null,
                                    "is_author_original_poster": true,
                                    "is_viewer_comment_poster": false,
                                    "is_author_bot": false,
                                    "is_author_non_coworker": false,
                                    "author_user_signals_renderer": {
                                        "__typename": "CometUFICommentActorUserSignalsRenderer",
                                        "user_signals_info": {
                                            "displayed_user_signals": [
                                                {
                                                    "id": "7332539900186091",
                                                    "signal_type_id": "325611522124903",
                                                    "lightModeImage": null,
                                                    "darkModeImage": null,
                                                    "tag_render_info": {
                                                        "comet_detail_view": null,
                                                        "color_variant": "PRIMARY",
                                                        "layout_type": "TEXT_ONLY"
                                                    },
                                                    "title": {
                                                        "text": "Tác giả"
                                                    }
                                                }
                                            ],
                                            "has_more": false,
                                            "overflow_uri": null,
                                            "total_count": 1,
                                            "show_middot": null
                                        },
                                        "__module_operation_CometUFICommentActorLinkBadges_comment": {
                                            "__dr": "CometUFICommentActorUserSignalsRenderer_renderer$normalization.graphql"
                                        },
                                        "__module_component_CometUFICommentActorLinkBadges_comment": {
                                            "__dr": "CometUFICommentActorUserSignalsRenderer.react"
                                        }
                                    },
                                    "author_badge_renderers": [],
                                    "identity_badges_web": [],
                                    "can_show_multiple_identity_badges": false,
                                    "discoverable_identity_badges_web": [],
                                    "user": {
                                        "name": "Le Hoang",
                                        "profile_picture": {
                                            "uri": "https://scontent.fsgn2-3.fna.fbcdn.net/v/t39.30808-1/386452053_303707972370995_1597759332350908646_n.jpg?stp=cp6_dst-jpg_p80x80&_nc_cat=107&ccb=1-7&_nc_sid=5f2048&_nc_ohc=BGHj1eJ8LxEAb5JjmGs&_nc_ht=scontent.fsgn2-3.fna&oh=00_AfACHQHYIgP20WahdtapSlsLS6CH0RSw09OrVY4PjC5ecg&oe=6622A178"
                                        },
                                        "id": "100081953824049"
                                    },
                                    "parent_post_story": {
                                        "attachments": [],
                                        "id": "UzpfSTEwMDA4MTk1MzgyNDA0OTpWSzo3NTI3ODg3OTI3MjMzMzgx"
                                    },
                                    "work_ama_answer_status": null,
                                    "work_knowledge_inline_annotation_comment_badge_renderer": null,
                                    "business_comment_attributes": [],
                                    "is_live_video_comment": false,
                                    "created_time": 1713024780,
                                    "translation_available_for_viewer": false,
                                    "inline_survey_config": null,
                                    "spam_display_mode": "none",
                                    "attached_story": null,
                                    "helpful_comments_comment_eyebrow_renderer": null,
                                    "comment_direct_parent": null,
                                    "if_viewer_can_see_member_page_tooltip": null,
                                    "is_disabled": false,
                                    "work_answered_event_comment_renderer": null,
                                    "comment_upper_badge_renderer": null,
                                    "elevated_comment_data": null,
                                    "__typename": "Comment"
                                },
                                "cursor": null
                            },
                            {
                                "node": {
                                    "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1MzQ3MDU2MzY1NTE2MTA=",
                                    "feedback": {
                                        "id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTM0NzA1NjM2NTUxNjEw",
                                        "expansion_info": {
                                            "expansion_token": "MjoxNzEzMTcxMTYwOgF18NfeqRMzJ7tITaVwdmpG7z7l9AR44Btpypw2hP9E9dW1st-2TCTUkem1I00JTz-Lvt_5Si-h2kwxbOy9vUYLfjMSYkCLD4tKvLrrvXbXctU3IMUHxws3yCOHB7xT6lw9nDAUi84IwJlf3mYrGvqJQSE2MpIubGpSWbSCj-Y2Ae-UcA2pEH6Mlho0fpfSbs4TnA6COspALB3Np20jOMCRci9jQ-1fwU7gv0LQJ_4eo1WLIoXg9j9qJjW6f8rPfO52qPaDCDWwSZSygn0TDud2gxW3TaiVVL0gtHE1pIZYN98iKd1mUwPUtS_Lgp8Z0MLyYTwepYRKGDanovRIssbpCkw8U1Q-j0YIqyDAE18YL3_Xbciy9VMNV2UzUyjNkB37OdBJaNlaUB55Yw8fz2RA7y5FSwft7tOjv0takNqm-gaIQjuoN36ZCcjE5VTeY48mYgfHf6NKp4nC9kc1yFrpqf0jU_p6ZCZAM4W6L3L3LrT9szEeICOk_Fgc_RvrBwfvN1yyx-gj_a1AAao",
                                            "should_show_reply_count": true
                                        },
                                        "replies_fields": {
                                            "filtering_footer_string": "",
                                            "count": 0,
                                            "total_count": 0
                                        },
                                        "viewer_actor": {
                                            "__typename": "User",
                                            "id": "61557504676830",
                                            "__isActor": "User",
                                            "name": "Lý Mai",
                                            "profile_picture_depth_0": {
                                                "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t1.30497-1/143086968_2856368904622192_1959732218791162458_n.png?stp=cp0_dst-png_p48x48&_nc_cat=1&ccb=1-7&_nc_sid=5f2048&_nc_ohc=kNSgHQLZ6doAb7eTDui&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDEoIPJUkx_mGovM_J3326vyBlc9auyJo-PJ_EBTtGgRg&oe=66445C78"
                                            },
                                            "profile_picture_depth_1": {
                                                "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t1.30497-1/143086968_2856368904622192_1959732218791162458_n.png?stp=cp0_dst-png_p40x40&_nc_cat=1&ccb=1-7&_nc_sid=5f2048&_nc_ohc=kNSgHQLZ6doAb7eTDui&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDqYKF91_-oKl07Nqn6ibjv0dysE8eyQkwL7oXXxsmLDA&oe=66445C78"
                                            },
                                            "gender": "MALE"
                                        },
                                        "url": "https://www.facebook.com/groups/autocsharp/posts/7527887927233381/?comment_id=7534705636551610",
                                        "__typename": "Feedback",
                                        "plugins": [
                                            {
                                                "__typename": "CommentComposerGroupMentionsPlugin",
                                                "group_id": "1777766135578951",
                                                "post_id": "7534705636551610",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerGroupMentionsPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerGroupMentionsPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerAvatarPlugin",
                                                "has_avatar": false,
                                                "feedback_id": "7534705636551610",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerAvatarPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerAvatarPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerHashtagPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerHashtagPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerHashtagPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerEmojiPlugin",
                                                "emoji_size": 16,
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerEmojiPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerEmojiPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerMediaUploadPlugin",
                                                "viewer_actor": {
                                                    "__typename": "User",
                                                    "id": "61557504676830"
                                                },
                                                "should_condense_video_preview": true,
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerMediaUploadPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerMediaUploadPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerGIFPlugin",
                                                "feedback_id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTM0NzA1NjM2NTUxNjEw",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerGIFPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerGIFPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CometComposerCometizedStickersPlugin",
                                                "feedback_id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTM0NzA1NjM2NTUxNjEw",
                                                "owning_profile_id": "100016882322080",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerStickersPlugin_next_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerStickersPlugin.next"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerEmoticonPlugin",
                                                "emoji_size": 16,
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerEmoticonPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerEmoticonPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerPrefillMentionPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerPrefillMentionPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerPrefillMentionPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerAssociateReplyWithParentPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerAssociateReplyWithParentPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerAssociateReplyWithParentPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerSetReplyClickedPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerSetReplyClickedPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerSetReplyClickedPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerStateSnapshotPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerStateSnapshotPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerStateSnapshotPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerLiveTypingBroadcastPlugin",
                                                "feedback_id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTM0NzA1NjM2NTUxNjEw",
                                                "viewer_actor": {
                                                    "__typename": "User",
                                                    "id": "61557504676830"
                                                },
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerLiveTypingBroadcastPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerLiveTypingBroadcastPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerCommentCharacterLimitPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerCommentCharacterLimitPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerCommentCharacterLimitPlugin"
                                                }
                                            },
                                            {
                                                "__typename": "CommentComposerWriteToComposerPlugin",
                                                "__module_operation_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerWriteToComposerPlugin_plugin$normalization.graphql"
                                                },
                                                "__module_component_useCometUFIComposerPlugins_feedback": {
                                                    "__dr": "cometUFIComposerWriteToComposerPlugin"
                                                }
                                            }
                                        ],
                                        "comment_composer_placeholder": "Viết phản hồi công khai…",
                                        "can_viewer_comment": true,
                                        "constituent_badge_banner_renderer": null,
                                        "have_comments_been_disabled": false,
                                        "are_live_video_comments_disabled": false,
                                        "is_viewer_muted": false,
                                        "total_comment_count": 0,
                                        "comments_disabled_notice_renderer": {
                                            "__typename": "GeneralCommentDisableNotice",
                                            "notice_message": {
                                                "delight_ranges": [],
                                                "image_ranges": [],
                                                "inline_style_ranges": [],
                                                "aggregated_ranges": [],
                                                "ranges": [],
                                                "color_ranges": [],
                                                "text": "Bình luận đã bị tắt cho bài viết này."
                                            },
                                            "__module_operation_CometUFICommentDisabledNotice_feedback": {
                                                "__dr": "CometGenericCommentDisableNotice_commentDisableNotice$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentDisabledNotice_feedback": {
                                                "__dr": "CometGenericCommentDisableNotice.react"
                                            }
                                        },
                                        "replies_connection": {
                                            "edges": [],
                                            "page_info": {
                                                "end_cursor": null,
                                                "has_next_page": false,
                                                "has_previous_page": false,
                                                "start_cursor": null
                                            }
                                        },
                                        "parent_object_ent": {
                                            "__typename": "Comment",
                                            "inline_replies_expander_renderer": null,
                                            "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1MzQ3MDU2MzY1NTE2MTA="
                                        },
                                        "viewer_feedback_reaction_info": null,
                                        "top_reactions": {
                                            "edges": []
                                        },
                                        "reactors": {
                                            "count_reduced": "0",
                                            "count": 0
                                        },
                                        "can_see_top_custom_reactions_on_comment_for_creators": null,
                                        "should_show_top_reactions": false
                                    },
                                    "legacy_fbid": "7534705636551610",
                                    "depth": 0,
                                    "body": {
                                        "text": "Buget bao nhiêu",
                                        "ranges": []
                                    },
                                    "attachments": [],
                                    "is_markdown_enabled": false,
                                    "community_comment_signal_renderer": null,
                                    "comment_menu_tooltip": "Ẩn hoặc báo cáo bình luận này",
                                    "should_show_comment_menu": true,
                                    "author": {
                                        "__typename": "User",
                                        "id": "100016882322080",
                                        "name": "Bodhi David",
                                        "__isActor": "User",
                                        "profile_picture_depth_0": {
                                            "uri": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.30808-1/329225074_577575460952465_7982256295253157376_n.jpg?stp=c19.0.48.48a_cp0_dst-jpg_p48x48&_nc_cat=102&ccb=1-7&_nc_sid=5f2048&_nc_ohc=STd7dDPJRsMAb6_seC4&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfDC6lD52mozLubpy86S0zWFret6Xm7JbldT5SaGxR6Q8w&oe=6622C43A"
                                        },
                                        "profile_picture_depth_1": {
                                            "uri": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.30808-1/329225074_577575460952465_7982256295253157376_n.jpg?stp=c16.0.40.40a_cp0_dst-jpg_p40x40&_nc_cat=102&ccb=1-7&_nc_sid=5f2048&_nc_ohc=STd7dDPJRsMAb6_seC4&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfCSrMSmfpo8DVhZf6JIPX2MiN6JomJ6CLb3IXHkGi_viA&oe=6622C43A"
                                        },
                                        "gender": "MALE",
                                        "__isEntity": "User",
                                        "url": "https://www.facebook.com/spady.horizon",
                                        "work_info": null,
                                        "is_verified": false,
                                        "short_name": "Bodhi",
                                        "subscribe_status": "CAN_SUBSCRIBE"
                                    },
                                    "is_author_weak_reference": false,
                                    "comment_action_links": [
                                        {
                                            "__typename": "XFBCommentTimeStampActionLink",
                                            "comment": {
                                                "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1MzQ3MDU2MzY1NTE2MTA=",
                                                "created_time": 1713169285,
                                                "url": "https://www.facebook.com/groups/autocsharp/posts/7527887927233381/?comment_id=7534705636551610"
                                            },
                                            "__module_operation_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentTimeStampActionLink_commentActionLink$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentTimeStampActionLink.react"
                                            }
                                        },
                                        {
                                            "__typename": "XFBCommentReactionActionLink",
                                            "comment": {
                                                "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1MzQ3MDU2MzY1NTE2MTA=",
                                                "is_live_video_comment": false,
                                                "feedback": {
                                                    "id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTM0NzA1NjM2NTUxNjEw",
                                                    "viewer_feedback_reaction_info": null,
                                                    "viewer_actor": {
                                                        "__typename": "User",
                                                        "id": "61557504676830"
                                                    },
                                                    "supported_reaction_infos": [
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An_NYk94x95Kypus5FJQ4k1oKEtko7-rUveEhwXytks318UoxoopBczHucoGDTjX4YcuAmIDkUw9SWBKhz7XYoAsQO_zxmWdkseO4YNdrvYmnIdmeAk.kf?ccb=10-5&oh=00_AfC4N59wnCTXy-mqcto-H4aFf0t_dEdWoIbTiBnBpDEN0A&oe=66447038&_nc_sid=7da55a"
                                                            },
                                                            "id": "1635855486666999"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9Tph7xL5aYi3BTTpVl2ow-l1vEv0-qYrBxereq6t6fWgcNnxeyJLsd3DuGnbCLdLFmcvvxn5ivo85wlrIv-EZhT1EucYZ-qoMW0ahYWHGpBBoqSjw.kf?ccb=10-5&oh=00_AfDQ-6lecXmTlchQ-RyfLcosRP1EUCa4krksCPKuOdWCvw&oe=66444D81&_nc_sid=7da55a"
                                                            },
                                                            "id": "1678524932434102"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An-iEpi04A6D-3XVq3wsUCtKdkB4w6IdurXeouCv4FsHYljtXw-fLrmbfC8B8zH5fPrckxLdEzR7V7dfidlNcrNoGsJWxiPDnzyNK-npl_KrJieMlg.kf?ccb=10-5&oh=00_AfAfoDjoOK-htcJ9ZDVYLBbUr_TNAdP_o_8P-R59OVhhig&oe=664475AE&_nc_sid=7da55a"
                                                            },
                                                            "id": "613557422527858"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9yyyXsW_c8BzV1_m0x9WqIPc7IKsshuStlldoUJeshdwMKRkmQmdPEGGwMopV9sH85YDKihkJ8DjNhx1wb2IaUuEOGzE_ji5F9MEXs_50bbA-IXQ.kf?ccb=10-5&oh=00_AfDHdIX2WR5sWRP3EbJwkmXXizlWvkkxyozcLRGko3OFmw&oe=664454A5&_nc_sid=7da55a"
                                                            },
                                                            "id": "115940658764963"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9Ob_EAguyCtqplSNOuikWQ6JjlxIh8vYoEgMXvR0CwneLvNdYwV-1NZgwJfR4aZ4QXhIpQUZxunwGdGubGw20jp-9DikfLbRVh-i4tobncZg9LGpE.kf?ccb=10-5&oh=00_AfBH4f_8b9YpKyqgriHL1hsfvrjLf57CHW4C13NN_Uqp1g&oe=66444171&_nc_sid=7da55a"
                                                            },
                                                            "id": "478547315650144"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9UFu6eXdDopP-SnPAhX-9SngOH_VeoYgHIGK6re6qbARX_PMcNl8Z14QPPFnVzbcfOQwxJxX5q-H5Fy3602EbOrVHhr1m4VSMXypn3fj2NSJongRg.kf?ccb=10-5&oh=00_AfDcHEN-Lj4ZCyxGPwBZoihFPCZSsZd9ZUgr77Gp74G5ag&oe=664467C8&_nc_sid=7da55a"
                                                            },
                                                            "id": "908563459236466"
                                                        },
                                                        {
                                                            "animation": {
                                                                "uri_keyframes2": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An919EwtdC17ceBi2men2TIR0UhNUwitUvpE61_Jbs44ggFt3mvLWkKiHP_CSmw72ohKdyEscSIBof6y1FeS57I3kGfh5tg96jndT5mnnEuJlpXuvuUj.kf?ccb=10-5&oh=00_AfD72uYo4bK4mUP0nsihQdCNdL-Eo6WbQt4XeEsX2z2zjw&oe=664465A4&_nc_sid=7da55a"
                                                            },
                                                            "id": "444813342392137"
                                                        }
                                                    ],
                                                    "if_viewer_can_use_creator_custom_reactions": null,
                                                    "associated_video": null,
                                                    "top_reactions": {
                                                        "edges": []
                                                    },
                                                    "unified_reactors": {
                                                        "count": 0
                                                    },
                                                    "reactors": {
                                                        "count": 0,
                                                        "is_empty": true
                                                    },
                                                    "if_viewer_can_render_creator_custom_reactions": null
                                                }
                                            },
                                            "__module_operation_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentReactionActionLink_commentActionLink$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentReactionActionLink.react"
                                            }
                                        },
                                        {
                                            "__typename": "XFBCommentReplyActionLink",
                                            "comment": {
                                                "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1MzQ3MDU2MzY1NTE2MTA=",
                                                "is_live_video_comment": false,
                                                "comment_parent": null,
                                                "is_author_weak_reference": false,
                                                "legacy_fbid": "7534705636551610",
                                                "url": "https://www.facebook.com/groups/autocsharp/posts/7527887927233381/?comment_id=7534705636551610",
                                                "author": {
                                                    "__typename": "User",
                                                    "id": "100016882322080",
                                                    "name": "Bodhi David",
                                                    "url": "https://www.facebook.com/spady.horizon"
                                                },
                                                "feedback": {
                                                    "comment_composer_placeholder": "Viết phản hồi công khai…",
                                                    "id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MV83NTM0NzA1NjM2NTUxNjEw"
                                                }
                                            },
                                            "__module_operation_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentReplyActionLink_commentActionLink$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentReplyActionLink.react"
                                            }
                                        },
                                        {
                                            "__typename": "XFBCommentShareActionLink",
                                            "comment": {
                                                "id": "Y29tbWVudDo3NTI3ODg3OTI3MjMzMzgxXzc1MzQ3MDU2MzY1NTE2MTA=",
                                                "url": "https://www.facebook.com/groups/autocsharp/posts/7527887927233381/?comment_id=7534705636551610",
                                                "__isEntity": "Comment",
                                                "__isNode": "Comment"
                                            },
                                            "__module_operation_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentShareActionLinkExperimental_commentActionLink$normalization.graphql"
                                            },
                                            "__module_component_CometUFICommentActionLinks_comment": {
                                                "__dr": "CometUFICommentShareActionLinkExperimental.react"
                                            }
                                        }
                                    ],
                                    "preferred_body": {
                                        "__typename": "TextWithEntities",
                                        "delight_ranges": [],
                                        "image_ranges": [],
                                        "inline_style_ranges": [],
                                        "aggregated_ranges": [],
                                        "ranges": [],
                                        "color_ranges": [],
                                        "text": "Buget bao nhiêu",
                                        "translation_type": "ORIGINAL"
                                    },
                                    "body_renderer": {
                                        "__typename": "TextWithEntities",
                                        "delight_ranges": [],
                                        "image_ranges": [],
                                        "inline_style_ranges": [],
                                        "aggregated_ranges": [],
                                        "ranges": [],
                                        "color_ranges": [],
                                        "text": "Buget bao nhiêu",
                                        "__module_operation_CometUFICommentTextBodyRenderer_comment": {
                                            "__dr": "CometUFICommentBodyTextWithEntities_textWithEntities$normalization.graphql"
                                        },
                                        "__module_component_CometUFICommentTextBodyRenderer_comment": {
                                            "__dr": "CometUFICommentBodyTextWithEntities.react"
                                        }
                                    },
                                    "comment_parent": null,
                                    "is_declined_by_group_admin_assistant": false,
                                    "is_gaming_video_comment": false,
                                    "timestamp_in_video": null,
                                    "translatability_for_viewer": {
                                        "source_dialect": "vi_VN"
                                    },
                                    "written_while_video_was_live": false,
                                    "group_comment_info": {
                                        "group": {
                                            "id": "1777766135578951",
                                            "answer_agent_id": null
                                        },
                                        "is_author_with_member_profile": true,
                                        "__module_operation_CometUFICommentActorLink_comment_groups": {
                                            "__dr": "CometUFIGroupCommentActorLink_groupCommentInfo$normalization.graphql"
                                        },
                                        "__module_component_CometUFICommentActorLink_comment_groups": {
                                            "__dr": "CometUFIGroupCommentActorLink.react"
                                        }
                                    },
                                    "bizweb_comment_info": null,
                                    "has_constituent_badge": false,
                                    "can_viewer_see_subsribe_button": false,
                                    "can_see_constituent_badge_upsell": false,
                                    "legacy_token": "7527887927233381_7534705636551610",
                                    "parent_feedback": {
                                        "id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MQ==",
                                        "share_fbid": "7527887927233381",
                                        "political_figure_data": null,
                                        "owning_profile": {
                                            "__typename": "User",
                                            "name": "Le Hoang",
                                            "id": "100081953824049"
                                        }
                                    },
                                    "question_and_answer_type": null,
                                    "is_author_original_poster": false,
                                    "is_viewer_comment_poster": false,
                                    "is_author_bot": false,
                                    "is_author_non_coworker": false,
                                    "author_user_signals_renderer": null,
                                    "author_badge_renderers": [],
                                    "identity_badges_web": [],
                                    "can_show_multiple_identity_badges": false,
                                    "discoverable_identity_badges_web": [],
                                    "user": {
                                        "name": "Bodhi David",
                                        "profile_picture": {
                                            "uri": "https://scontent.fsgn2-8.fna.fbcdn.net/v/t39.30808-1/329225074_577575460952465_7982256295253157376_n.jpg?stp=c32.0.80.80a_cp0_dst-jpg_p80x80&_nc_cat=102&ccb=1-7&_nc_sid=5f2048&_nc_ohc=STd7dDPJRsMAb6_seC4&_nc_ht=scontent.fsgn2-8.fna&oh=00_AfDTHhHVZdNWNw4q73w21jkS3HVNdLYunmLw0NYr4xo7EA&oe=6622C43A"
                                        },
                                        "id": "100016882322080"
                                    },
                                    "parent_post_story": {
                                        "attachments": [],
                                        "id": "UzpfSTEwMDA4MTk1MzgyNDA0OTpWSzo3NTI3ODg3OTI3MjMzMzgx"
                                    },
                                    "work_ama_answer_status": null,
                                    "work_knowledge_inline_annotation_comment_badge_renderer": null,
                                    "business_comment_attributes": [],
                                    "is_live_video_comment": false,
                                    "created_time": 1713169285,
                                    "translation_available_for_viewer": false,
                                    "inline_survey_config": null,
                                    "spam_display_mode": "none",
                                    "attached_story": null,
                                    "helpful_comments_comment_eyebrow_renderer": null,
                                    "comment_direct_parent": null,
                                    "if_viewer_can_see_member_page_tooltip": null,
                                    "is_disabled": false,
                                    "work_answered_event_comment_renderer": null,
                                    "comment_upper_badge_renderer": null,
                                    "elevated_comment_data": null,
                                    "__typename": "Comment"
                                },
                                "cursor": null
                            }
                        ],
                        "page_info": {
                            "end_cursor": "AQHR91U-JVOAxz5r-v8alGUmeruXzr8qAPXwIUldx8UYnj_R-rc26JwqVgZWEk6NZnFlzzrn8r_V1PXItHv7DbYzjw",
                            "has_next_page": false,
                            "has_previous_page": false,
                            "start_cursor": "AQHRAW_qd9-RotmXYBMw-nMiTxhRWEcqQM7y9Y5YJKtZwU1hXPpWxkkkEQN9r0WMfOag9gAnmZarmb94Y8m9uJv_6g"
                        }
                    }
                },
                "typing_indicator_renderer": null,
                "viewer_actor": {
                    "__typename": "User",
                    "id": "61557504676830",
                    "__isActor": "User",
                    "name": "Lý Mai",
                    "profile_picture_depth_0": {
                        "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t1.30497-1/143086968_2856368904622192_1959732218791162458_n.png?stp=cp0_dst-png_p48x48&_nc_cat=1&ccb=1-7&_nc_sid=5f2048&_nc_ohc=kNSgHQLZ6doAb7eTDui&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDEoIPJUkx_mGovM_J3326vyBlc9auyJo-PJ_EBTtGgRg&oe=66445C78"
                    },
                    "profile_picture_depth_1": {
                        "uri": "https://scontent.fsgn2-11.fna.fbcdn.net/v/t1.30497-1/143086968_2856368904622192_1959732218791162458_n.png?stp=cp0_dst-png_p40x40&_nc_cat=1&ccb=1-7&_nc_sid=5f2048&_nc_ohc=kNSgHQLZ6doAb7eTDui&_nc_ht=scontent.fsgn2-11.fna&oh=00_AfDqYKF91_-oKl07Nqn6ibjv0dysE8eyQkwL7oXXxsmLDA&oe=66445C78"
                    },
                    "gender": "MALE"
                },
                "url": "https://www.facebook.com/groups/autocsharp/permalink/7527887927233381/",
                "plugins": [
                    {
                        "__typename": "CommentComposerGroupMentionsPlugin",
                        "group_id": "1777766135578951",
                        "post_id": "7527887927233381",
                        "__module_operation_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerGroupMentionsPlugin_plugin$normalization.graphql"
                        },
                        "__module_component_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerGroupMentionsPlugin"
                        }
                    },
                    {
                        "__typename": "CommentComposerAvatarPlugin",
                        "has_avatar": false,
                        "feedback_id": "7527887927233381",
                        "__module_operation_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerAvatarPlugin_plugin$normalization.graphql"
                        },
                        "__module_component_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerAvatarPlugin"
                        }
                    },
                    {
                        "__typename": "CommentComposerHashtagPlugin",
                        "__module_operation_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerHashtagPlugin_plugin$normalization.graphql"
                        },
                        "__module_component_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerHashtagPlugin"
                        }
                    },
                    {
                        "__typename": "CommentComposerEmojiPlugin",
                        "emoji_size": 16,
                        "__module_operation_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerEmojiPlugin_plugin$normalization.graphql"
                        },
                        "__module_component_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerEmojiPlugin"
                        }
                    },
                    {
                        "__typename": "CommentComposerMediaUploadPlugin",
                        "viewer_actor": {
                            "__typename": "User",
                            "id": "61557504676830"
                        },
                        "should_condense_video_preview": true,
                        "__module_operation_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerMediaUploadPlugin_plugin$normalization.graphql"
                        },
                        "__module_component_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerMediaUploadPlugin"
                        }
                    },
                    {
                        "__typename": "CommentComposerGIFPlugin",
                        "feedback_id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MQ==",
                        "__module_operation_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerGIFPlugin_plugin$normalization.graphql"
                        },
                        "__module_component_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerGIFPlugin"
                        }
                    },
                    {
                        "__typename": "CometComposerCometizedStickersPlugin",
                        "feedback_id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MQ==",
                        "owning_profile_id": "100081953824049",
                        "__module_operation_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerStickersPlugin_next_plugin$normalization.graphql"
                        },
                        "__module_component_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerStickersPlugin.next"
                        }
                    },
                    {
                        "__typename": "CommentComposerEmoticonPlugin",
                        "emoji_size": 16,
                        "__module_operation_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerEmoticonPlugin_plugin$normalization.graphql"
                        },
                        "__module_component_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerEmoticonPlugin"
                        }
                    },
                    {
                        "__typename": "CommentComposerPrefillMentionPlugin",
                        "__module_operation_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerPrefillMentionPlugin_plugin$normalization.graphql"
                        },
                        "__module_component_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerPrefillMentionPlugin"
                        }
                    },
                    {
                        "__typename": "CommentComposerAssociateReplyWithParentPlugin",
                        "__module_operation_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerAssociateReplyWithParentPlugin_plugin$normalization.graphql"
                        },
                        "__module_component_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerAssociateReplyWithParentPlugin"
                        }
                    },
                    {
                        "__typename": "CommentComposerSetReplyClickedPlugin",
                        "__module_operation_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerSetReplyClickedPlugin_plugin$normalization.graphql"
                        },
                        "__module_component_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerSetReplyClickedPlugin"
                        }
                    },
                    {
                        "__typename": "CommentComposerStateSnapshotPlugin",
                        "__module_operation_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerStateSnapshotPlugin_plugin$normalization.graphql"
                        },
                        "__module_component_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerStateSnapshotPlugin"
                        }
                    },
                    {
                        "__typename": "CommentComposerLiveTypingBroadcastPlugin",
                        "feedback_id": "ZmVlZGJhY2s6NzUyNzg4NzkyNzIzMzM4MQ==",
                        "viewer_actor": {
                            "__typename": "User",
                            "id": "61557504676830"
                        },
                        "__module_operation_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerLiveTypingBroadcastPlugin_plugin$normalization.graphql"
                        },
                        "__module_component_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerLiveTypingBroadcastPlugin"
                        }
                    },
                    {
                        "__typename": "CommentComposerCommentCharacterLimitPlugin",
                        "__module_operation_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerCommentCharacterLimitPlugin_plugin$normalization.graphql"
                        },
                        "__module_component_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerCommentCharacterLimitPlugin"
                        }
                    },
                    {
                        "__typename": "CommentComposerWriteToComposerPlugin",
                        "__module_operation_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerWriteToComposerPlugin_plugin$normalization.graphql"
                        },
                        "__module_component_useCometUFIComposerPlugins_feedback": {
                            "__dr": "cometUFIComposerWriteToComposerPlugin"
                        }
                    }
                ],
                "comment_composer_placeholder": "Viết câu trả lời...",
                "can_viewer_comment": true,
                "constituent_badge_banner_renderer": null,
                "have_comments_been_disabled": false,
                "are_live_video_comments_disabled": false,
                "is_viewer_muted": false,
                "comments_disabled_notice_renderer": {
                    "__typename": "GeneralCommentDisableNotice",
                    "notice_message": {
                        "delight_ranges": [],
                        "image_ranges": [],
                        "inline_style_ranges": [],
                        "aggregated_ranges": [],
                        "ranges": [],
                        "color_ranges": [],
                        "text": "Bình luận đã bị tắt cho bài viết này."
                    },
                    "__module_operation_CometUFICommentDisabledNotice_feedback": {
                        "__dr": "CometGenericCommentDisableNotice_commentDisableNotice$normalization.graphql"
                    },
                    "__module_component_CometUFICommentDisabledNotice_feedback": {
                        "__dr": "CometGenericCommentDisableNotice.react"
                    }
                }
            }
        },
        "extensions": {
            "is_final": true,
            "sr_payload": {
                "ddd": {
                    "hsrp": {
                        "hsdp": {
                            "clpData": {
                                "1743656": {
                                    "r": 1
                                },
                                "1744251": {
                                    "r": 100,
                                    "s": 1
                                },
                                "1836368": {
                                    "r": 1,
                                    "s": 1
                                },
                                "6181": {
                                    "r": 1,
                                    "s": 1
                                },
                                "1814852": {
                                    "r": 1
                                },
                                "1828945": {
                                    "r": 100,
                                    "s": 1
                                },
                                "1837559": {
                                    "r": 1
                                },
                                "1838142": {
                                    "r": 1,
                                    "s": 1
                                },
                                "1848815": {
                                    "r": 10000,
                                    "s": 1
                                },
                                "1962341": {
                                    "r": 1,
                                    "s": 1
                                },
                                "4405": {
                                    "r": 1
                                },
                                "1744178": {
                                    "r": 1,
                                    "s": 1
                                },
                                "4883": {
                                    "r": 1,
                                    "s": 1
                                },
                                "2132": {
                                    "r": 1
                                },
                                "2133": {
                                    "r": 1
                                },
                                "445": {
                                    "r": 1
                                },
                                "446": {
                                    "r": 1
                                },
                                "447": {
                                    "r": 1
                                },
                                "2646": {
                                    "r": 1,
                                    "s": 1
                                },
                                "2647": {
                                    "r": 1,
                                    "s": 1
                                },
                                "2648": {
                                    "r": 1,
                                    "s": 1
                                },
                                "2649": {
                                    "r": 1,
                                    "s": 1
                                },
                                "2650": {
                                    "r": 1,
                                    "s": 1
                                },
                                "2651": {
                                    "r": 1,
                                    "s": 1
                                },
                                "3766": {
                                    "r": 1,
                                    "s": 1
                                },
                                "1968720": {
                                    "r": 1,
                                    "s": 1
                                },
                                "4652": {
                                    "r": 1000,
                                    "s": 1
                                },
                                "5519": {
                                    "r": 100,
                                    "s": 1
                                },
                                "1743356": {
                                    "r": 1
                                },
                                "1985969": {
                                    "r": 10,
                                    "s": 1
                                },
                                "1744057": {
                                    "r": 500,
                                    "s": 1
                                },
                                "1744058": {
                                    "r": 5000,
                                    "s": 1
                                },
                                "1744059": {
                                    "r": 10000,
                                    "s": 1
                                },
                                "1744060": {
                                    "r": 1000,
                                    "s": 1
                                },
                                "1744247": {
                                    "r": 1
                                },
                                "1744249": {
                                    "r": 1
                                },
                                "819": {
                                    "r": 1,
                                    "s": 1
                                },
                                "1857112": {
                                    "r": 1
                                },
                                "1755537": {
                                    "r": 1
                                },
                                "2": {
                                    "r": 1,
                                    "s": 1
                                },
                                "20": {
                                    "r": 1,
                                    "s": 1
                                },
                                "1497": {
                                    "r": 1
                                },
                                "4274": {
                                    "r": 1
                                },
                                "4275": {
                                    "r": 1,
                                    "s": 1
                                },
                                "5721": {
                                    "r": 1,
                                    "s": 1
                                },
                                "5722": {
                                    "r": 1,
                                    "s": 1
                                },
                                "5723": {
                                    "r": 1,
                                    "s": 1
                                },
                                "5727": {
                                    "r": 1,
                                    "s": 1
                                },
                                "1956659": {
                                    "r": 1
                                }
                            },
                            "gkxData": {
                                "7742": {
                                    "result": false,
                                    "hash": null
                                },
                                "20836": {
                                    "result": false,
                                    "hash": null
                                },
                                "20935": {
                                    "result": true,
                                    "hash": null
                                },
                                "20936": {
                                    "result": true,
                                    "hash": null
                                },
                                "20939": {
                                    "result": true,
                                    "hash": null
                                },
                                "21074": {
                                    "result": false,
                                    "hash": null
                                },
                                "1167": {
                                    "result": false,
                                    "hash": "AT6T2-4bAiLB5Y6xLZk"
                                },
                                "21050": {
                                    "result": false,
                                    "hash": null
                                },
                                "24283": {
                                    "result": false,
                                    "hash": null
                                },
                                "21059": {
                                    "result": false,
                                    "hash": null
                                },
                                "22813": {
                                    "result": false,
                                    "hash": null
                                },
                                "23874": {
                                    "result": true,
                                    "hash": null
                                },
                                "20942": {
                                    "result": false,
                                    "hash": null
                                },
                                "21003": {
                                    "result": false,
                                    "hash": null
                                },
                                "21004": {
                                    "result": false,
                                    "hash": null
                                },
                                "21005": {
                                    "result": false,
                                    "hash": null
                                },
                                "21093": {
                                    "result": false,
                                    "hash": null
                                },
                                "21095": {
                                    "result": false,
                                    "hash": null
                                },
                                "22878": {
                                    "result": true,
                                    "hash": null
                                },
                                "22879": {
                                    "result": false,
                                    "hash": null
                                },
                                "22968": {
                                    "result": false,
                                    "hash": null
                                },
                                "23405": {
                                    "result": true,
                                    "hash": null
                                },
                                "23406": {
                                    "result": false,
                                    "hash": null
                                },
                                "23407": {
                                    "result": false,
                                    "hash": null
                                },
                                "23554": {
                                    "result": true,
                                    "hash": null
                                },
                                "24215": {
                                    "result": false,
                                    "hash": null
                                },
                                "24216": {
                                    "result": false,
                                    "hash": null
                                },
                                "26210": {
                                    "result": false,
                                    "hash": null
                                },
                                "21086": {
                                    "result": false,
                                    "hash": null
                                },
                                "21087": {
                                    "result": false,
                                    "hash": null
                                },
                                "21088": {
                                    "result": false,
                                    "hash": null
                                },
                                "21089": {
                                    "result": false,
                                    "hash": null
                                },
                                "21090": {
                                    "result": true,
                                    "hash": null
                                },
                                "21091": {
                                    "result": true,
                                    "hash": null
                                },
                                "329": {
                                    "result": false,
                                    "hash": null
                                },
                                "847": {
                                    "result": true,
                                    "hash": null
                                },
                                "22681": {
                                    "result": false,
                                    "hash": null
                                },
                                "22773": {
                                    "result": false,
                                    "hash": null
                                },
                                "22785": {
                                    "result": false,
                                    "hash": null
                                },
                                "22803": {
                                    "result": false,
                                    "hash": null
                                },
                                "22826": {
                                    "result": false,
                                    "hash": null
                                },
                                "22827": {
                                    "result": true,
                                    "hash": null
                                },
                                "22875": {
                                    "result": false,
                                    "hash": null
                                },
                                "22876": {
                                    "result": true,
                                    "hash": null
                                },
                                "22877": {
                                    "result": true,
                                    "hash": null
                                },
                                "26334": {
                                    "result": false,
                                    "hash": null
                                },
                                "20940": {
                                    "result": false,
                                    "hash": null
                                },
                                "21043": {
                                    "result": false,
                                    "hash": null
                                },
                                "21118": {
                                    "result": true,
                                    "hash": null
                                },
                                "20921": {
                                    "result": true,
                                    "hash": null
                                },
                                "20922": {
                                    "result": true,
                                    "hash": null
                                },
                                "20923": {
                                    "result": true,
                                    "hash": null
                                },
                                "20924": {
                                    "result": true,
                                    "hash": null
                                },
                                "20925": {
                                    "result": true,
                                    "hash": null
                                },
                                "20926": {
                                    "result": true,
                                    "hash": null
                                },
                                "20927": {
                                    "result": true,
                                    "hash": null
                                },
                                "20928": {
                                    "result": true,
                                    "hash": null
                                },
                                "25572": {
                                    "result": false,
                                    "hash": null
                                },
                                "196": {
                                    "result": false,
                                    "hash": null
                                },
                                "209": {
                                    "result": false,
                                    "hash": null
                                },
                                "1154": {
                                    "result": false,
                                    "hash": null
                                },
                                "1181": {
                                    "result": false,
                                    "hash": null
                                },
                                "1514": {
                                    "result": false,
                                    "hash": null
                                },
                                "20979": {
                                    "result": false,
                                    "hash": null
                                },
                                "20980": {
                                    "result": true,
                                    "hash": null
                                },
                                "20981": {
                                    "result": false,
                                    "hash": null
                                },
                                "20982": {
                                    "result": false,
                                    "hash": null
                                },
                                "20983": {
                                    "result": true,
                                    "hash": null
                                },
                                "20984": {
                                    "result": true,
                                    "hash": null
                                },
                                "20985": {
                                    "result": false,
                                    "hash": null
                                },
                                "20986": {
                                    "result": false,
                                    "hash": null
                                },
                                "20987": {
                                    "result": false,
                                    "hash": null
                                },
                                "20988": {
                                    "result": true,
                                    "hash": null
                                },
                                "21075": {
                                    "result": false,
                                    "hash": null
                                },
                                "21076": {
                                    "result": true,
                                    "hash": null
                                },
                                "21106": {
                                    "result": true,
                                    "hash": null
                                },
                                "21107": {
                                    "result": false,
                                    "hash": null
                                },
                                "21117": {
                                    "result": false,
                                    "hash": null
                                },
                                "22792": {
                                    "result": false,
                                    "hash": null
                                },
                                "22979": {
                                    "result": false,
                                    "hash": null
                                },
                                "23433": {
                                    "result": false,
                                    "hash": null
                                },
                                "26340": {
                                    "result": false,
                                    "hash": null
                                },
                                "26341": {
                                    "result": false,
                                    "hash": null
                                },
                                "26342": {
                                    "result": false,
                                    "hash": null
                                },
                                "943": {
                                    "result": false,
                                    "hash": null
                                },
                                "24279": {
                                    "result": false,
                                    "hash": null
                                },
                                "24280": {
                                    "result": false,
                                    "hash": null
                                },
                                "24281": {
                                    "result": false,
                                    "hash": null
                                },
                                "24282": {
                                    "result": false,
                                    "hash": null
                                },
                                "22812": {
                                    "result": true,
                                    "hash": null
                                },
                                "550": {
                                    "result": false,
                                    "hash": null
                                },
                                "1326": {
                                    "result": false,
                                    "hash": null
                                },
                                "24298": {
                                    "result": false,
                                    "hash": null
                                },
                                "24319": {
                                    "result": false,
                                    "hash": null
                                },
                                "24565": {
                                    "result": false,
                                    "hash": null
                                },
                                "1624": {
                                    "result": false,
                                    "hash": null
                                },
                                "21051": {
                                    "result": false,
                                    "hash": null
                                },
                                "21052": {
                                    "result": false,
                                    "hash": null
                                },
                                "21053": {
                                    "result": false,
                                    "hash": null
                                },
                                "21054": {
                                    "result": false,
                                    "hash": null
                                },
                                "21055": {
                                    "result": false,
                                    "hash": null
                                },
                                "21056": {
                                    "result": false,
                                    "hash": null
                                },
                                "21057": {
                                    "result": false,
                                    "hash": null
                                },
                                "21058": {
                                    "result": true,
                                    "hash": null
                                },
                                "23403": {
                                    "result": false,
                                    "hash": null
                                },
                                "23404": {
                                    "result": true,
                                    "hash": null
                                },
                                "22802": {
                                    "result": false,
                                    "hash": null
                                },
                                "3416": {
                                    "result": false,
                                    "hash": null
                                },
                                "20864": {
                                    "result": true,
                                    "hash": null
                                },
                                "20865": {
                                    "result": true,
                                    "hash": null
                                },
                                "23413": {
                                    "result": false,
                                    "hash": null
                                },
                                "23414": {
                                    "result": false,
                                    "hash": null
                                },
                                "23229": {
                                    "result": false,
                                    "hash": null
                                },
                                "23231": {
                                    "result": false,
                                    "hash": null
                                },
                                "23280": {
                                    "result": true,
                                    "hash": "AT4Pz3mzIUeCtHRNXbo"
                                },
                                "25978": {
                                    "result": false,
                                    "hash": null
                                },
                                "21096": {
                                    "result": false,
                                    "hash": null
                                },
                                "21119": {
                                    "result": false,
                                    "hash": null
                                },
                                "21120": {
                                    "result": false,
                                    "hash": null
                                },
                                "21121": {
                                    "result": false,
                                    "hash": null
                                },
                                "21122": {
                                    "result": false,
                                    "hash": null
                                },
                                "21123": {
                                    "result": false,
                                    "hash": null
                                },
                                "21124": {
                                    "result": false,
                                    "hash": null
                                },
                                "20915": {
                                    "result": false,
                                    "hash": null
                                },
                                "20916": {
                                    "result": true,
                                    "hash": null
                                },
                                "20917": {
                                    "result": false,
                                    "hash": null
                                },
                                "20918": {
                                    "result": false,
                                    "hash": null
                                },
                                "20919": {
                                    "result": true,
                                    "hash": null
                                },
                                "20920": {
                                    "result": false,
                                    "hash": null
                                },
                                "20929": {
                                    "result": true,
                                    "hash": null
                                },
                                "26332": {
                                    "result": true,
                                    "hash": null
                                },
                                "9999": {
                                    "result": false,
                                    "hash": null
                                },
                                "23245": {
                                    "result": false,
                                    "hash": null
                                },
                                "366": {
                                    "result": false,
                                    "hash": "AT4tZUu5NKh7yD_YiEg"
                                },
                                "7329": {
                                    "result": false,
                                    "hash": null
                                },
                                "9861": {
                                    "result": true,
                                    "hash": null
                                },
                                "20858": {
                                    "result": true,
                                    "hash": null
                                },
                                "20859": {
                                    "result": false,
                                    "hash": null
                                },
                                "20860": {
                                    "result": true,
                                    "hash": null
                                },
                                "20863": {
                                    "result": false,
                                    "hash": null
                                },
                                "21062": {
                                    "result": false,
                                    "hash": null
                                },
                                "21063": {
                                    "result": false,
                                    "hash": null
                                },
                                "21065": {
                                    "result": true,
                                    "hash": "AT78i2s-oKvPyc7-suI"
                                },
                                "21069": {
                                    "result": false,
                                    "hash": null
                                },
                                "21071": {
                                    "result": false,
                                    "hash": null
                                },
                                "21072": {
                                    "result": false,
                                    "hash": null
                                },
                                "33056": {
                                    "result": false,
                                    "hash": null
                                },
                                "20976": {
                                    "result": false,
                                    "hash": null
                                },
                                "20977": {
                                    "result": false,
                                    "hash": null
                                },
                                "21037": {
                                    "result": false,
                                    "hash": null
                                },
                                "23906": {
                                    "result": false,
                                    "hash": null
                                },
                                "24028": {
                                    "result": true,
                                    "hash": null
                                },
                                "24032": {
                                    "result": false,
                                    "hash": null
                                },
                                "26364": {
                                    "result": true,
                                    "hash": null
                                }
                            },
                            "ixData": {
                                "478231": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 12,
                                    "h": 12,
                                    "p": "0 -914px",
                                    "sz": "26px 998px"
                                },
                                "550098": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -1188px",
                                    "sz": "26px 1522px"
                                },
                                "568448": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -1422px",
                                    "sz": "26px 1522px"
                                },
                                "642536": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -1242px",
                                    "sz": "26px 1522px"
                                },
                                "687980": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -1278px",
                                    "sz": "26px 1522px"
                                },
                                "687986": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -1404px",
                                    "sz": "26px 1522px"
                                },
                                "1704745": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -1152px",
                                    "sz": "26px 1522px"
                                },
                                "502062": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -252px",
                                    "sz": "26px 998px"
                                },
                                "1876411": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/y3/r/yr1yU4iRD3j.gif",
                                    "width": 12,
                                    "height": 12
                                },
                                "1876412": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/y_/r/gechF9FUhlA.gif",
                                    "width": 16,
                                    "height": 16
                                },
                                "1876413": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yj/r/GWhjF42XFxf.gif",
                                    "width": 20,
                                    "height": 20
                                },
                                "1876414": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/y7/r/enJRxtt-UCR.gif",
                                    "width": 24,
                                    "height": 24
                                },
                                "1876415": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yS/r/VWAJZQFF-Id.gif",
                                    "width": 32,
                                    "height": 32
                                },
                                "1876416": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yh/r/CvaXg0xMrcV.gif",
                                    "width": 48,
                                    "height": 48
                                },
                                "1876418": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/y3/r/GSd71G0jO4k.gif",
                                    "width": 72,
                                    "height": 72
                                },
                                "1876419": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/y_/r/hFhIPpP61ko.gif",
                                    "width": 12,
                                    "height": 12
                                },
                                "1876420": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yU/r/mFgfn_gyAJ1.gif",
                                    "width": 16,
                                    "height": 16
                                },
                                "1876421": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yM/r/InyICizOHBi.gif",
                                    "width": 20,
                                    "height": 20
                                },
                                "1876422": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/y4/r/U1PQVaq7RlN.gif",
                                    "width": 24,
                                    "height": 24
                                },
                                "1876423": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yP/r/98RswzXXP_l.gif",
                                    "width": 32,
                                    "height": 32
                                },
                                "1876424": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/y6/r/jBq3e5arNdc.gif",
                                    "width": 48,
                                    "height": 48
                                },
                                "1876426": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yb/r/5SUwhSIaYPi.gif",
                                    "width": 72,
                                    "height": 72
                                },
                                "1876427": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yC/r/eWzMyB55EM9.gif",
                                    "width": 12,
                                    "height": 12
                                },
                                "1876428": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/y-/r/UZBgfIHrBWr.gif",
                                    "width": 16,
                                    "height": 16
                                },
                                "1876429": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yI/r/1bRE9cbjn1b.gif",
                                    "width": 20,
                                    "height": 20
                                },
                                "1876430": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yU/r/aY9rUjW6Knt.gif",
                                    "width": 24,
                                    "height": 24
                                },
                                "1876431": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yV/r/saqH5viFdeS.gif",
                                    "width": 32,
                                    "height": 32
                                },
                                "1876432": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yE/r/II5Zz_xyaRq.gif",
                                    "width": 48,
                                    "height": 48
                                },
                                "1876434": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/y6/r/ZiYCx8qFFeS.gif",
                                    "width": 72,
                                    "height": 72
                                },
                                "1876435": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yC/r/HlfX2g7BKQF.gif",
                                    "width": 12,
                                    "height": 12
                                },
                                "1876436": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yA/r/FgCYwBPJQbD.gif",
                                    "width": 16,
                                    "height": 16
                                },
                                "1876437": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/y5/r/Tk5Nsxzl5uN.gif",
                                    "width": 20,
                                    "height": 20
                                },
                                "1876438": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yg/r/sZfWhK12sK9.gif",
                                    "width": 24,
                                    "height": 24
                                },
                                "1876439": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yY/r/YldUjsQY4ip.gif",
                                    "width": 32,
                                    "height": 32
                                },
                                "1876440": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yi/r/C2iup3gA8gj.gif",
                                    "width": 48,
                                    "height": 48
                                },
                                "1876442": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yC/r/b1Afiy8wHIx.gif",
                                    "width": 72,
                                    "height": 72
                                },
                                "1876443": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yD/r/RRvdQ84ON5F.gif",
                                    "width": 12,
                                    "height": 12
                                },
                                "1876444": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/ys/r/_9f6LAHdTX8.gif",
                                    "width": 16,
                                    "height": 16
                                },
                                "1876445": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yz/r/wXmsdTeMbHA.gif",
                                    "width": 20,
                                    "height": 20
                                },
                                "1876446": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yh/r/MHI-ZasUNH3.gif",
                                    "width": 24,
                                    "height": 24
                                },
                                "1876447": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yd/r/0fZRJV0OxgA.gif",
                                    "width": 32,
                                    "height": 32
                                },
                                "1876448": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yQ/r/3rT1VhOamk_.gif",
                                    "width": 48,
                                    "height": 48
                                },
                                "1876450": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yY/r/u5mmCFJkZ86.gif",
                                    "width": 72,
                                    "height": 72
                                },
                                "1876451": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yL/r/i9Mx4pmHqlx.gif",
                                    "width": 12,
                                    "height": 12
                                },
                                "1876452": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yu/r/D0YJrEOUQPH.gif",
                                    "width": 16,
                                    "height": 16
                                },
                                "1876453": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yH/r/bykveQ2w6so.gif",
                                    "width": 20,
                                    "height": 20
                                },
                                "1876454": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yM/r/mn224E_W9XQ.gif",
                                    "width": 24,
                                    "height": 24
                                },
                                "1876455": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yo/r/vcQVEo1xDPT.gif",
                                    "width": 32,
                                    "height": 32
                                },
                                "1876456": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yO/r/jO8807KweBl.gif",
                                    "width": 48,
                                    "height": 48
                                },
                                "1876458": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/y9/r/fb2pjlVk4lg.gif",
                                    "width": 72,
                                    "height": 72
                                },
                                "1940508": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yQ/r/UpUSqVdIbF7.gif",
                                    "width": 64,
                                    "height": 64
                                },
                                "1940509": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yi/r/UmGPk6v4FkU.gif",
                                    "width": 60,
                                    "height": 60
                                },
                                "1940510": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yj/r/A4qg4fFBbio.gif",
                                    "width": 60,
                                    "height": 60
                                },
                                "1940511": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yN/r/lOdq_WbW0wR.gif",
                                    "width": 60,
                                    "height": 60
                                },
                                "1940512": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/yN/r/Y0ifOT9SKtG.gif",
                                    "width": 60,
                                    "height": 60
                                },
                                "1940513": {
                                    "sprited": 0,
                                    "uri": "https://static.xx.fbcdn.net/rsrc.php/v3/y6/r/XrctmjDeGXx.gif",
                                    "width": 60,
                                    "height": 60
                                },
                                "701592": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 8,
                                    "h": 8,
                                    "p": "-14px -872px",
                                    "sz": "26px 998px"
                                },
                                "702721": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 8,
                                    "h": 8,
                                    "p": "-14px -902px",
                                    "sz": "26px 998px"
                                },
                                "897949": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 8,
                                    "h": 8,
                                    "p": "-14px -892px",
                                    "sz": "26px 998px"
                                },
                                "1739808": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 8,
                                    "h": 8,
                                    "p": "-14px -882px",
                                    "sz": "26px 998px"
                                },
                                "491221": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 12,
                                    "h": 12,
                                    "p": "0 -942px",
                                    "sz": "26px 998px"
                                },
                                "491223": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -538px",
                                    "sz": "26px 998px"
                                },
                                "648667": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 12,
                                    "h": 12,
                                    "p": "0 -970px",
                                    "sz": "26px 998px"
                                },
                                "648669": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -626px",
                                    "sz": "26px 998px"
                                },
                                "14175": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -26px",
                                    "sz": "26px 1522px"
                                },
                                "111404": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -378px",
                                    "sz": "26px 1522px"
                                },
                                "111412": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -576px",
                                    "sz": "26px 1522px"
                                },
                                "111418": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -686px",
                                    "sz": "26px 1522px"
                                },
                                "111421": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -906px",
                                    "sz": "26px 1522px"
                                },
                                "347019": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 18,
                                    "h": 18,
                                    "p": "0 -1012px",
                                    "sz": "26px 1522px"
                                },
                                "347020": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 18,
                                    "h": 18,
                                    "p": "0 -1032px",
                                    "sz": "26px 1522px"
                                },
                                "347022": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 18,
                                    "h": 18,
                                    "p": "0 -1092px",
                                    "sz": "26px 1522px"
                                },
                                "352555": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 18,
                                    "h": 18,
                                    "p": "0 -1052px",
                                    "sz": "26px 1522px"
                                },
                                "352559": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 18,
                                    "h": 18,
                                    "p": "0 -1112px",
                                    "sz": "26px 1522px"
                                },
                                "386426": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -670px",
                                    "sz": "26px 998px"
                                },
                                "386427": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -730px",
                                    "sz": "26px 1522px"
                                },
                                "386428": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -752px",
                                    "sz": "26px 1522px"
                                },
                                "386429": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -774px",
                                    "sz": "26px 1522px"
                                },
                                "386436": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -796px",
                                    "sz": "26px 1522px"
                                },
                                "386438": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -818px",
                                    "sz": "26px 1522px"
                                },
                                "386439": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -840px",
                                    "sz": "26px 1522px"
                                },
                                "386622": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -598px",
                                    "sz": "26px 1522px"
                                },
                                "386749": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -950px",
                                    "sz": "26px 1522px"
                                },
                                "387252": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -1458px",
                                    "sz": "26px 1522px"
                                },
                                "387254": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -1476px",
                                    "sz": "26px 1522px"
                                },
                                "389933": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -400px",
                                    "sz": "26px 1522px"
                                },
                                "389935": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -422px",
                                    "sz": "26px 1522px"
                                },
                                "389937": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -444px",
                                    "sz": "26px 1522px"
                                },
                                "389939": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -466px",
                                    "sz": "26px 1522px"
                                },
                                "389941": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -488px",
                                    "sz": "26px 1522px"
                                },
                                "389943": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -510px",
                                    "sz": "26px 1522px"
                                },
                                "389945": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -532px",
                                    "sz": "26px 1522px"
                                },
                                "389947": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -554px",
                                    "sz": "26px 1522px"
                                },
                                "389949": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -620px",
                                    "sz": "26px 1522px"
                                },
                                "389951": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -642px",
                                    "sz": "26px 1522px"
                                },
                                "389953": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -664px",
                                    "sz": "26px 1522px"
                                },
                                "389955": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -708px",
                                    "sz": "26px 1522px"
                                },
                                "389957": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -862px",
                                    "sz": "26px 1522px"
                                },
                                "389959": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -884px",
                                    "sz": "26px 1522px"
                                },
                                "478237": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -764px",
                                    "sz": "26px 998px"
                                },
                                "481767": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -312px",
                                    "sz": "26px 1522px"
                                },
                                "484391": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 24,
                                    "h": 24,
                                    "p": "0 -156px",
                                    "sz": "26px 998px"
                                },
                                "484394": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -836px",
                                    "sz": "26px 998px"
                                },
                                "484398": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -1350px",
                                    "sz": "26px 1522px"
                                },
                                "484399": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 18,
                                    "h": 18,
                                    "p": "0 -1132px",
                                    "sz": "26px 1522px"
                                },
                                "484757": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -296px",
                                    "sz": "26px 998px"
                                },
                                "484865": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -1296px",
                                    "sz": "26px 1522px"
                                },
                                "485103": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -246px",
                                    "sz": "26px 1522px"
                                },
                                "487090": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -334px",
                                    "sz": "26px 1522px"
                                },
                                "487562": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -202px",
                                    "sz": "26px 1522px"
                                },
                                "487626": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -290px",
                                    "sz": "26px 1522px"
                                },
                                "490501": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -70px",
                                    "sz": "26px 1522px"
                                },
                                "491230": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -1260px",
                                    "sz": "26px 1522px"
                                },
                                "492454": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -340px",
                                    "sz": "26px 998px"
                                },
                                "492488": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -114px",
                                    "sz": "26px 1522px"
                                },
                                "492518": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -362px",
                                    "sz": "26px 998px"
                                },
                                "492521": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 24,
                                    "h": 24,
                                    "p": "0 -78px",
                                    "sz": "26px 998px"
                                },
                                "492536": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -384px",
                                    "sz": "26px 998px"
                                },
                                "492572": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -406px",
                                    "sz": "26px 998px"
                                },
                                "492575": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 24,
                                    "h": 24,
                                    "p": "0 -104px",
                                    "sz": "26px 998px"
                                },
                                "497241": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -92px",
                                    "sz": "26px 1522px"
                                },
                                "498146": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -274px",
                                    "sz": "26px 998px"
                                },
                                "498857": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -136px",
                                    "sz": "26px 1522px"
                                },
                                "505565": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -428px",
                                    "sz": "26px 998px"
                                },
                                "505620": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -48px",
                                    "sz": "26px 1522px"
                                },
                                "507176": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -158px",
                                    "sz": "26px 1522px"
                                },
                                "508557": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -1224px",
                                    "sz": "26px 1522px"
                                },
                                "508558": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 18,
                                    "h": 18,
                                    "p": "0 -972px",
                                    "sz": "26px 1522px"
                                },
                                "509922": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 18,
                                    "h": 18,
                                    "p": "0 -992px",
                                    "sz": "26px 1522px"
                                },
                                "509926": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 18,
                                    "h": 18,
                                    "p": "0 -1072px",
                                    "sz": "26px 1522px"
                                },
                                "512647": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -208px",
                                    "sz": "26px 998px"
                                },
                                "514454": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -230px",
                                    "sz": "26px 998px"
                                },
                                "545517": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -472px",
                                    "sz": "26px 998px"
                                },
                                "559830": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -224px",
                                    "sz": "26px 1522px"
                                },
                                "621399": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -450px",
                                    "sz": "26px 998px"
                                },
                                "659288": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -648px",
                                    "sz": "26px 998px"
                                },
                                "679141": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -356px",
                                    "sz": "26px 1522px"
                                },
                                "1478524": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -1170px",
                                    "sz": "26px 1522px"
                                },
                                "484385": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 12,
                                    "h": 12,
                                    "p": "0 -928px",
                                    "sz": "26px 998px"
                                },
                                "481880": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 12,
                                    "h": 12,
                                    "p": "0 -984px",
                                    "sz": "26px 998px"
                                },
                                "481882": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -854px",
                                    "sz": "26px 998px"
                                },
                                "478232": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -746px",
                                    "sz": "26px 998px"
                                },
                                "657883": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -1386px",
                                    "sz": "26px 1522px"
                                },
                                "1937973": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/33uRJSkrOlX.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -1368px",
                                    "sz": "26px 1522px"
                                },
                                "492485": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -710px",
                                    "sz": "26px 998px"
                                },
                                "492533": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 16,
                                    "h": 16,
                                    "p": "0 -728px",
                                    "sz": "26px 998px"
                                },
                                "785426": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 12,
                                    "h": 12,
                                    "p": "0 -900px",
                                    "sz": "26px 998px"
                                },
                                "1664042": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 20,
                                    "h": 20,
                                    "p": "0 -604px",
                                    "sz": "26px 998px"
                                },
                                "506962": {
                                    "sprited": 2,
                                    "spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "_spi": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/AHolfQ2_wLa.png",
                                    "w": 12,
                                    "h": 12,
                                    "p": "0 -956px",
                                    "sz": "26px 998px"
                                }
                            },
                            "metaconfigData": {
                                "61": {
                                    "value": false
                                },
                                "15": {
                                    "value": false
                                },
                                "99": {
                                    "value": false
                                }
                            },
                            "qexData": {
                                "526": {
                                    "r": 250
                                },
                                "538": {
                                    "r": 5000
                                },
                                "543": {
                                    "r": 10000
                                },
                                "372": {
                                    "r": null
                                },
                                "662": {
                                    "r": null
                                },
                                "723": {
                                    "r": false
                                },
                                "68": {
                                    "r": true,
                                    "l": "J{\"u\":\"\",\"t\":\"fb\",\"gks\":[],\"qe\":null}"
                                },
                                "717": {
                                    "r": "none"
                                },
                                "762": {
                                    "r": "none"
                                },
                                "960": {
                                    "r": false
                                },
                                "1111": {
                                    "r": false
                                },
                                "301": {
                                    "r": true,
                                    "l": "J{\"u\":\"\",\"t\":\"fb_acting_account\",\"gks\":[],\"qe\":\"442443411778320\"}"
                                },
                                "881": {
                                    "r": true,
                                    "l": "J{\"u\":\"\",\"t\":\"fb_acting_account\",\"gks\":[],\"qe\":\"442443411778320\"}"
                                },
                                "1240": {
                                    "r": 1500
                                },
                                "576": {
                                    "r": 10,
                                    "l": "J{\"u\":\"\",\"t\":\"fb\",\"gks\":[],\"qe\":null}"
                                },
                                "617": {
                                    "r": 10,
                                    "l": "J{\"u\":\"\",\"t\":\"fb\",\"gks\":[],\"qe\":null}"
                                },
                                "1777": {
                                    "r": 10,
                                    "l": "J{\"u\":\"\",\"t\":\"fb\",\"gks\":[],\"qe\":null}"
                                },
                                "104": {
                                    "r": null
                                },
                                "128": {
                                    "r": 250
                                },
                                "344": {
                                    "r": 5000
                                },
                                "388": {
                                    "r": 5000
                                },
                                "644": {
                                    "r": null
                                },
                                "9": {
                                    "r": true
                                }
                            },
                            "qplData": {
                                "1217": {
                                    "r": 1
                                },
                                "2410": {
                                    "r": 1
                                },
                                "6204": {
                                    "r": 7
                                },
                                "6702": {
                                    "r": 1
                                },
                                "4750": {
                                    "r": 1
                                },
                                "54": {
                                    "r": 500
                                },
                                "232": {
                                    "r": 50
                                },
                                "622": {
                                    "r": 100
                                },
                                "702": {
                                    "r": 500
                                },
                                "1099": {
                                    "r": 1000
                                },
                                "1269": {
                                    "r": 1000
                                },
                                "1585": {
                                    "r": 1000
                                },
                                "1811": {
                                    "r": 100
                                },
                                "1891": {
                                    "r": 50
                                },
                                "2960": {
                                    "r": 1000
                                },
                                "3289": {
                                    "r": 1000
                                },
                                "3455": {
                                    "r": 100
                                },
                                "4690": {
                                    "r": 100
                                },
                                "4694": {
                                    "r": 10000
                                },
                                "5054": {
                                    "r": 1
                                },
                                "5737": {
                                    "r": 100
                                },
                                "5992": {
                                    "r": 50
                                },
                                "6043": {
                                    "r": 1000
                                },
                                "6153": {
                                    "r": 100
                                },
                                "6177": {
                                    "r": 100
                                },
                                "6752": {
                                    "r": 50
                                },
                                "6895": {
                                    "r": 10000
                                },
                                "7056": {
                                    "r": 50
                                },
                                "7109": {
                                    "r": 100
                                },
                                "7148": {
                                    "r": 50
                                },
                                "7493": {
                                    "r": 1000
                                },
                                "7813": {
                                    "r": 1
                                },
                                "4977": {
                                    "r": 4
                                },
                                "431": {},
                                "4389": {
                                    "r": 250
                                },
                                "112": {}
                            },
                            "justknobxData": {
                                "1845": {
                                    "r": true
                                },
                                "144": {
                                    "r": true
                                },
                                "450": {
                                    "r": true
                                },
                                "1203": {
                                    "r": true
                                },
                                "494": {
                                    "r": true
                                },
                                "2269": {
                                    "r": false
                                },
                                "55": {
                                    "r": true
                                },
                                "317": {
                                    "r": 16
                                },
                                "1023": {
                                    "r": true
                                }
                            }
                        },
                        "hblp": {
                            "consistency": {
                                "rev": 1012776817,
                                "actions": {
                                    "1": []
                                }
                            },
                            "rsrcMap": {
                                "v39gSxj": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/y9/r/NGk-fx6Kdj7.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main",
                                    "prelude": 1
                                },
                                "vhKfY5c": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iqm64/yv/l/makehaste_jhash/p8adCfpCHTP6s6IR6XA7FerqlJYNmLOEiahCbB2THXvaooMWJHk2rfkaXulZlOn1t4_KrxTEPQzCQcJsZrNGxt6CYHANu_6F2D5boHuHC-vu_85ajRQAhtdZOvQRYnuuvqkHuR693zE7wb9R5ecYCMZukYr5_PhZt9eSvY73LNuIVCmLA-uzeSOJBuYxsw_y3zVOBS78aJvWfi_KGCjKhH33iJ2Op55HfXW__mM.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iqo-4/y3/l/vi_VN/p8adCfpCHTP6s6IR6XA7FerqlJYNmLOEiahCbB2THXvaooMWJHk2rfkaXulZlOn1t4_KrxTEPQzCQcJsZrNGxt6CYHANu_6F2D5boHuHC-vu_85ajRQAhtdZOvQRYnuuvqkHuR693zE7wb9R5ecYCMZukYr5_PhZt9eSvY73LNuIVCmLA-uzeSOJBuYxsw_y3zVOBS78aJvWfi_KGCjKhH33iJ2Op55HfXW__mM.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "2hPt+8f": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iuOl4/yg/l/makehaste_jhash/-orIkj7rBwq.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iI0j4/y7/l/vi_VN/-orIkj7rBwq.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "UZfqf8J": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iESk4/yT/l/makehaste_jhash/FIrlppSo7CV.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6id664/yq/l/vi_VN/FIrlppSo7CV.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "cKZv3P8": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3i_IY4/ye/l/makehaste_jhash/9IkE98ncOsA.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6i-K_4/y9/l/vi_VN/9IkE98ncOsA.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "UX5ZaR7": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3isa44/yI/l/makehaste_jhash/DZbRJTZyBlz.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6inK84/yl/l/vi_VN/DZbRJTZyBlz.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "uLB6aZe": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/y2/r/4YvmlJKzjxE.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "eJ8EHGb": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yi/r/YeYg2e1RETb.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "QHlvoYy": {
                                    "type": "css",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yn/l/0,cross/GMAcg7L7j8MS8asBiucNgP.css?_nc_x=TYpZFU0ANEZ"
                                },
                                "4UiubQr": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yu/r/hZ5OUDUTAqA.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "AdpmZX+": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iQbs4/yF/l/makehaste_jhash/7X12msSBx5I.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iYuE4/y0/l/vi_VN/7X12msSBx5I.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "mbuNvlv": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iOo24/yc/l/makehaste_jhash/JEtN0WAqtCs.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iOo24/yX/l/vi_VN/JEtN0WAqtCs.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "tytAcfm": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yU/r/CgOdIT306TZ.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "mueC9mU": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yK/r/8K4A7soqX88.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "zdnyIKV": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3i-Vf4/yI/l/makehaste_jhash/jumcRz9_dVP.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6i0Qq4/y1/l/vi_VN/jumcRz9_dVP.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "nVZGLFA": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yW/r/dHX5-rbH-pj.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "7L5r4xF": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3i0Wo4/yh/l/makehaste_jhash/Gbe_EsNfcgJ.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iNbE4/ye/l/vi_VN/Gbe_EsNfcgJ.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "w0NV5zs": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yU/r/p_12XW-SeNk.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "19hbtN7": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3ioUt4/yU/l/makehaste_jhash/hyn52J2T4Pv.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iBt44/yf/l/vi_VN/hyn52J2T4Pv.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "BOv7jro": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yj/r/YDo2W_lUrxr.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "7CxomUC": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3i1i14/yk/l/makehaste_jhash/9hiQajIx8l2.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iAgK4/y7/l/vi_VN/9hiQajIx8l2.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "I9Os7/3": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/r/VawOpA8eZd_.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "ao/gvNJ": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yR/r/9cw7bGI1a2e.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "XogzSlm": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yC/r/oH36BB8a58v.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "p6J0Y88": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yR/r/ERz6pNGhHp8.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "x4h+czF": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yW/r/KEJ681csanv.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "yYKrU3b": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3i2fB4/y_/l/makehaste_jhash/6NjFs8U9P3F.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6it_84/y4/l/vi_VN/6NjFs8U9P3F.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "8zcMZlF": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yT/r/9pTHwj5mBY8.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "Qac+fS7": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yf/r/UTCI3tptf-1.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "TRZv/O7": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iZBT4/ya/l/makehaste_jhash/gY-zeqPgUGL.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iGgg4/yH/l/vi_VN/gY-zeqPgUGL.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "9/ZUyY7": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iraF4/yC/l/makehaste_jhash/mf2l7zpiVq5.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6ij_d4/yP/l/vi_VN/mf2l7zpiVq5.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "Chizidw": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iyNV4/y6/l/makehaste_jhash/5FxxDJ3lHrC.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iVZd4/yO/l/vi_VN/5FxxDJ3lHrC.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "I0yjxZj": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/ya/r/15Cs84Ic8LQ.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "NPjH0oN": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yB/r/RyufPx5Sr0t.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "armDlnN": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3igyD4/yh/l/makehaste_jhash/D2yiB0_wmRe.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iAnv4/yb/l/vi_VN/D2yiB0_wmRe.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "mFMciEA": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3ipNS4/y_/l/makehaste_jhash/JAx2404I8gK.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iXnA4/yL/l/vi_VN/JAx2404I8gK.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "pDVLiqo": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yM/r/guPPB-g1E6k.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "g3REIDt": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yn/r/pecttNl0AsH.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "RuadkF1": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yv/r/7xaRW_9U7Fg.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "ozIZ976": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3i5aJ4/yD/l/makehaste_jhash/1d3AbgRDn3l.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iVD24/yP/l/vi_VN/1d3AbgRDn3l.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "/Sf8nOw": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yx/r/RcUrBhGlkbD.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "eNG9XyS": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iOE14/yg/l/makehaste_jhash/aSF1MlhRxnc.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iS8B4/yV/l/vi_VN/aSF1MlhRxnc.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "5UILrzD": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yh/r/NpXVin1DLVt.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "mo2I/T0": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/y-/r/_g3OwPXx4xr.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "2/wduKH": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yw/r/z8B8xiDf1-g.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "LNCbLG/": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iwdk4/yg/l/makehaste_jhash/IGTjDTUFkIQ.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6ikqv4/yF/l/vi_VN/IGTjDTUFkIQ.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "NsUnhYF": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3if2L4/yz/l/makehaste_jhash/bUDFE5KIfud.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iY7a4/y9/l/vi_VN/bUDFE5KIfud.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "/fxotSe": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3i7M54/yi/l/makehaste_jhash/20arraLEdGZ.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iJ044/yJ/l/vi_VN/20arraLEdGZ.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "d8fl4DI": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yX/r/XCcuwXqLwkL.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "uvQp8p4": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yi/r/Tda60TB2HQ0.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "sD3z2ST": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/ys/r/OgQZKqBcuUW.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "5AbbSjw": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iSR44/yD/l/makehaste_jhash/rWs8JXkNdM4.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iyuK4/yq/l/vi_VN/rWs8JXkNdM4.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "Yh/JWiF": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/y9/r/oWHFlPWy_eg.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "LtG+1uG": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yo/r/Kr7NWzOpJfy.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "rR9pDGR": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yJ/r/biMJeUW8RES.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "pUpnrMq": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yq/r/XGzOnfTjEts.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "AlP3gQE": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yi/r/Im9fveCC02m.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "Fo8wih0": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yO/r/ObbJ9AIjbyB.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "kN8TgSz": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3ijrk4/yD/l/makehaste_jhash/klgj3vpvo-Y.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iqNt4/yN/l/vi_VN/klgj3vpvo-Y.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "FC9h7XN": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3ixKz4/yo/l/makehaste_jhash/P17j30LeOxA.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6izHu4/yf/l/vi_VN/P17j30LeOxA.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "gHB6UlN": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3ib674/ys/l/makehaste_jhash/8QuUEhEHLF6.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iQVr4/yI/l/vi_VN/8QuUEhEHLF6.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "mNoT6/f": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iYOw4/yt/l/makehaste_jhash/oP0U3-DLN2L.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iefr4/yJ/l/vi_VN/oP0U3-DLN2L.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "21zJ1Og": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iytJ4/yZ/l/makehaste_jhash/OaRdK6I3N0R.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6i0mz4/yL/l/vi_VN/OaRdK6I3N0R.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "Opz2BIO": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3ivVi4/yA/l/makehaste_jhash/FGtioyZkGIp.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6i63V4/yi/l/vi_VN/FGtioyZkGIp.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "gxxmBEY": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yU/r/7Cmf2UdEvCO.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "mFOUf9V": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3ieKI4/yi/l/makehaste_jhash/klqyXfWh6fC.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iecS4/y4/l/vi_VN/klqyXfWh6fC.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "q293ET7": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yO/r/qBzwIsjl30S.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "f4wal+l": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yL/r/xOCAVNdb1JV.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "nhm6xwY": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/y1/r/QRsTXKojc3W.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "8LWPrbs": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yy/r/Th9IWHQ9Kmt.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "a/IJsf4": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yU/r/61sqkWOuVxG.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "+SU8cpz": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yG/r/hbNcTYCNOCJ.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "+uA+HvV": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yH/r/McmmlgNgQpj.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "OjGdplo": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/y7/r/ahtiUXJ0jFQ.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "7fNe6yM": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yO/r/U2a72jI1O09.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_longtail"
                                },
                                "U952axk": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iYzh4/yZ/l/makehaste_jhash/AW6IMxjgOP9.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iAfp4/yh/l/vi_VN/AW6IMxjgOP9.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "Lx/GDfZ": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yz/r/bjflaViwk4g.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "YBTqXQg": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iTlT4/yt/l/makehaste_jhash/PtWwkX5HVUG.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6ielb4/yg/l/vi_VN/PtWwkX5HVUG.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "iHcJp2L": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yL/r/47YkFgeivhh.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "mv0ik3v": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/y_/r/W6kto9oLDaf.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_longtail"
                                },
                                "iLDhQqa": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3i7gr4/yo/l/makehaste_jhash/LRD4KADtQU2.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iHmt4/yO/l/vi_VN/LRD4KADtQU2.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "ZDahxXw": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yC/r/ZNr-0gh15GX.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "wBHmF39": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iuY84/y7/l/makehaste_jhash/zcQ0-Ojrfsv.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iT7Z4/yL/l/vi_VN/zcQ0-Ojrfsv.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "wyTDu/+": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/y1/r/b0XVSUJLW7b.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "3xZAcjl": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yC/r/c6abdKqNRP2.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "KrvVkDS": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3i6zW4/yZ/l/makehaste_jhash/Wt1e-SueJTL.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iWoc4/yC/l/vi_VN/Wt1e-SueJTL.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "+kuUnwE": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yy/r/5r1v89-9txa.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "/KCWsjQ": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yw/r/zck1CkeA6l7.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "NFfKbD8": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3i5K-4/y-/l/makehaste_jhash/BemPeD87mvv.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iDOI4/yS/l/vi_VN/BemPeD87mvv.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "q3tcYA4": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yI/r/-PCklPiZAS0.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "bSfLrme": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3ipQq4/yp/l/makehaste_jhash/g9qgq9MO7G8.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6ivYG4/yK/l/vi_VN/g9qgq9MO7G8.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "r5UmZvF": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yE/r/iEvjq2iS4hD.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_longtail"
                                },
                                "92FWu0u": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yZ/r/VZTLT8Vxml6.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_longtail"
                                },
                                "7iemgNg": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iVsn4/ya/l/makehaste_jhash/InaeCBW8TTO.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iYuq4/yL/l/vi_VN/InaeCBW8TTO.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "qZrkqYZ": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iVAb4/yj/l/makehaste_jhash/yIllFY4e6_g.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iUhT4/yu/l/vi_VN/yIllFY4e6_g.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_longtail"
                                },
                                "KpspYp1": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/S3rXyQpTMip.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "dPhs+py": {
                                    "type": "css",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/y0/l/0,cross/qqmTb9tpO1G.css?_nc_x=TYpZFU0ANEZ"
                                },
                                "p8R/8l/": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yi/r/aiIwK4dUW85.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "fxI9l/Y": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3i5FB4/y7/l/makehaste_jhash/w5j64w7yMHb.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iHdQ4/y-/l/vi_VN/w5j64w7yMHb.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "SF5a4/N": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3ivl74/ys/l/makehaste_jhash/NNSBr2qZXMk.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iKYu4/y2/l/vi_VN/NNSBr2qZXMk.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "X81AtpF": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iHES4/yl/l/makehaste_jhash/JdbMQ94UQP_.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iDP34/yx/l/vi_VN/JdbMQ94UQP_.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "XndYMPP": {
                                    "type": "css",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yD/l/0,cross/zyEpb6SJKFF.css?_nc_x=TYpZFU0ANEZ"
                                },
                                "wqwDtIe": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3if0w4/yk/l/makehaste_jhash/YqxBbtIEXUI.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6i9zV4/y9/l/vi_VN/YqxBbtIEXUI.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "TQMvJ5Y": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3indV4/yW/l/makehaste_jhash/vuDiwesUoRL.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6i2RH4/yO/l/vi_VN/vuDiwesUoRL.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "n1/Vx7b": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iCXF4/yC/l/makehaste_jhash/NZDVHgetJC_.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iu074/yA/l/vi_VN/NZDVHgetJC_.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "ALBhwn6": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iDyq4/yo/l/makehaste_jhash/-2go0pRCevf.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iD2z4/yI/l/vi_VN/-2go0pRCevf.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "WpvFyQK": {
                                    "type": "css",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yp/l/0,cross/lN0ZymlTe3X.css?_nc_x=TYpZFU0ANEZ"
                                },
                                "oi7cBD/": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iIU54/yf/l/makehaste_jhash/ybYL7fb_fRA.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iu5l4/yG/l/vi_VN/ybYL7fb_fRA.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "Qr223WB": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yz/r/NNmFb9xPEbF.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "X2lXaqk": {
                                    "type": "css",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/y4/l/0,cross/WPrndevEYn8.css?_nc_x=TYpZFU0ANEZ"
                                },
                                "8sg2K08": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3i_vm4/yK/l/makehaste_jhash/PWXxL6XhHd2.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iEuE4/yz/l/vi_VN/PWXxL6XhHd2.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "2aWc0ax": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iTRp4/yy/l/makehaste_jhash/ZN01nQovzRz.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6i4pv4/yq/l/vi_VN/ZN01nQovzRz.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "Na1E3Dy": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3i5Un4/ym/l/makehaste_jhash/Lu1UoPS9SBY.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iiJR4/yu/l/vi_VN/Lu1UoPS9SBY.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_longtail"
                                },
                                "CJ7ZV8+": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iJRj4/y0/l/makehaste_jhash/9wAvjY3GEHr.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iyQw4/yQ/l/vi_VN/9wAvjY3GEHr.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_longtail"
                                },
                                "1eL6p1Q": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3ibti4/yI/l/makehaste_jhash/OG1jLa0aJCg.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iNGl4/yG/l/vi_VN/OG1jLa0aJCg.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "I+GHswV": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yS/r/ui2DkP-wt_7.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "R/kfhPG": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iGlx4/yP/l/makehaste_jhash/75kT_6x9fZT.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iiFh4/yf/l/vi_VN/75kT_6x9fZT.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "84Rk5n3": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3ixqs4/yZ/l/makehaste_jhash/ekC1sCejClR.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iXhI4/ye/l/vi_VN/ekC1sCejClR.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "W+TDAGO": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yX/r/yeOH4X6mS8A.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "mw2Kc1Z": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3i_Ww4/yC/l/makehaste_jhash/h-KEtWYGm6n.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6i0sd4/yE/l/vi_VN/h-KEtWYGm6n.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_longtail"
                                },
                                "/NTWV2I": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3ipLN4/yl/l/makehaste_jhash/-7jQZj14qNY.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6ijgG4/yf/l/vi_VN/-7jQZj14qNY.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_longtail"
                                },
                                "ZmGgkXA": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yE/r/e9COMMAHpJ-.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "KKqBUon": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iFqW4/yB/l/makehaste_jhash/DIdHneTMXc4.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iMk-4/yd/l/vi_VN/DIdHneTMXc4.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "6CoHJPY": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iLl54/y6/l/makehaste_jhash/kgRPo2u1q0L.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iWPy4/yt/l/vi_VN/kgRPo2u1q0L.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "7z1tgPR": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3i7fB4/yT/l/makehaste_jhash/oKHiVhTtNOu.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6ibaa4/yy/l/vi_VN/oKHiVhTtNOu.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "jPMYVE1": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3ii-T4/y6/l/makehaste_jhash/XbhwI1uQi8C.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iO324/yz/l/vi_VN/XbhwI1uQi8C.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "XnjZlAC": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iHOv4/yL/l/makehaste_jhash/uXeE2r3JcHI.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6izee4/yI/l/vi_VN/uXeE2r3JcHI.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "CMrhgpl": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yj/r/Lo5cFOH43BP.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "gI8i2t+": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yt/r/aa8NGAwcPRy.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "tSjPifJ": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iRxL4/yz/l/makehaste_jhash/AHfJCsOMg1J.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6i7X24/yp/l/vi_VN/AHfJCsOMg1J.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "LpbHyFh": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yA/r/sfAUB_WuLV0.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "RpwSNth": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3ijqY4/ys/l/makehaste_jhash/1zATV3sJIpm.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iGuD4/yI/l/vi_VN/1zATV3sJIpm.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "nlR+S3x": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yV/r/IuoLI1241bd.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "Bw4pRwt": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iEuQ4/yk/l/makehaste_jhash/bNoaPUAoo2s.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6iBHR4/yk/l/vi_VN/bNoaPUAoo2s.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_longtail"
                                },
                                "/b5dsuK": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yo/r/72kZU-_RCFh.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "GfZQS3k": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/ys/r/Bp1d3gkbH2u.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_longtail"
                                },
                                "oCMPVVY": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yj/r/y8mAeviUiFU.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_longtail"
                                },
                                "mFkoxEV": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yT/r/MuVJ3kziB_s.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "A8Zmczg": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yl/r/kZJA7p6AQCs.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_longtail"
                                },
                                "eMxoRDZ": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yr/r/dSqE-FQFvAX.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_longtail"
                                },
                                "inDZbxT": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/y7/r/Z6oo2PNyPUl.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "lqR6G6x": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yq/r/pF4Iattwin0.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "v2p0ZYx": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/y4/r/R0Qk0mB-FqU.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "V0egoaT": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yu/r/il3R1k7d8Yf.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                },
                                "CMzu9iV": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/y5/r/ha33Gtj2G8o.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_longtail"
                                },
                                "qAifaaj": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3/yo/r/iKMdSHsqsTi.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_longtail"
                                },
                                "jipJXH1": {
                                    "type": "js",
                                    "src": "https://static.xx.fbcdn.net/rsrc.php/v3iBF_4/yn/l/makehaste_jhash/Ezdgww5P0mY.js?_nc_x=TYpZFU0ANEZ",
                                    "tsrc": "https://static.xx.fbcdn.net/rsrc-translations.php/v6i8Nm4/yW/l/vi_VN/Ezdgww5P0mY.js?_nc_x=TYpZFU0ANEZ",
                                    "m": "1012776817_main"
                                }
                            },
                            "compMap": {
                                "CometUFIAvatarPopoverForLexical.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "AdpmZX+",
                                        "yYKrU3b",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "8zcMZlF",
                                        "cKZv3P8",
                                        "UX5ZaR7",
                                        "uLB6aZe",
                                        "Qac+fS7",
                                        "eJ8EHGb",
                                        "QHlvoYy",
                                        "TRZv/O7",
                                        "mbuNvlv",
                                        "4UiubQr",
                                        "tytAcfm"
                                    ],
                                    "rdfds": {
                                        "m": [
                                            "CometExceptionDialog.react",
                                            "FDSTooltipDeferredImpl.react"
                                        ]
                                    },
                                    "rds": {
                                        "m": [
                                            "ContextualConfig",
                                            "BladeRunnerClient",
                                            "CometToast.react",
                                            "MAWMICSafe",
                                            "FbtLogging",
                                            "DGWRequestStreamClient",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent",
                                            "CometRelayEF",
                                            "MqttLongPollingRunner"
                                        ],
                                        "r": [
                                            "BOv7jro",
                                            "7CxomUC",
                                            "I9Os7/3",
                                            "mueC9mU"
                                        ]
                                    },
                                    "be": 1
                                },
                                "CometUFIEmojiPickerPopoverForLexical.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "AdpmZX+",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "9/ZUyY7",
                                        "UX5ZaR7",
                                        "uLB6aZe",
                                        "Chizidw",
                                        "eJ8EHGb",
                                        "I0yjxZj",
                                        "QHlvoYy",
                                        "2hPt+8f",
                                        "mbuNvlv",
                                        "4UiubQr",
                                        "NPjH0oN",
                                        "tytAcfm"
                                    ],
                                    "rds": {
                                        "m": [
                                            "FbtLogging",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent"
                                        ]
                                    },
                                    "be": 1
                                },
                                "CometUFIMediaUploadUpgradedPlugin.experimental.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "AdpmZX+",
                                        "armDlnN",
                                        "mFMciEA",
                                        "pDVLiqo",
                                        "g3REIDt",
                                        "UZfqf8J",
                                        "RuadkF1",
                                        "ozIZ976",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "/Sf8nOw",
                                        "UX5ZaR7",
                                        "eNG9XyS",
                                        "5UILrzD",
                                        "mo2I/T0",
                                        "uLB6aZe",
                                        "2/wduKH",
                                        "Chizidw",
                                        "LNCbLG/",
                                        "NsUnhYF",
                                        "eJ8EHGb",
                                        "/fxotSe",
                                        "QHlvoYy",
                                        "d8fl4DI",
                                        "uvQp8p4",
                                        "2hPt+8f",
                                        "sD3z2ST",
                                        "5AbbSjw",
                                        "Yh/JWiF",
                                        "LtG+1uG",
                                        "rR9pDGR",
                                        "pUpnrMq",
                                        "mbuNvlv",
                                        "tytAcfm"
                                    ],
                                    "rdfds": {
                                        "m": [
                                            "CometExceptionDialog.react",
                                            "FDSTooltipDeferredImpl.react"
                                        ]
                                    },
                                    "rds": {
                                        "m": [
                                            "ContextualConfig",
                                            "BladeRunnerClient",
                                            "FbtLogging",
                                            "DGWRequestStreamClient",
                                            "CometSuspenseFalcoEvent",
                                            "ODS",
                                            "IntlQtEventFalcoEvent",
                                            "MqttLongPollingRunner",
                                            "CometToast.react",
                                            "MAWMICSafe",
                                            "CometRelayEF"
                                        ],
                                        "r": [
                                            "BOv7jro",
                                            "7CxomUC",
                                            "I9Os7/3",
                                            "mueC9mU"
                                        ]
                                    },
                                    "be": 1
                                },
                                "CometUFIGIFPickerPopoverForLexical.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "AdpmZX+",
                                        "AlP3gQE",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "UX5ZaR7",
                                        "Fo8wih0",
                                        "kN8TgSz",
                                        "uLB6aZe",
                                        "FC9h7XN",
                                        "Qac+fS7",
                                        "eJ8EHGb",
                                        "gHB6UlN",
                                        "QHlvoYy",
                                        "uvQp8p4",
                                        "mbuNvlv",
                                        "tytAcfm"
                                    ],
                                    "rdfds": {
                                        "m": [
                                            "CometExceptionDialog.react",
                                            "FDSTooltipDeferredImpl.react"
                                        ]
                                    },
                                    "rds": {
                                        "m": [
                                            "FbtLogging",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent"
                                        ]
                                    },
                                    "be": 1
                                },
                                "CometStickerPickerCard.react": {
                                    "r": [
                                        "mNoT6/f",
                                        "vhKfY5c",
                                        "21zJ1Og",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "8zcMZlF",
                                        "cKZv3P8",
                                        "UX5ZaR7",
                                        "eNG9XyS",
                                        "kN8TgSz",
                                        "uLB6aZe",
                                        "LNCbLG/",
                                        "Qac+fS7",
                                        "eJ8EHGb",
                                        "gHB6UlN",
                                        "QHlvoYy",
                                        "2hPt+8f",
                                        "Opz2BIO",
                                        "mbuNvlv",
                                        "mueC9mU",
                                        "tytAcfm"
                                    ],
                                    "rdfds": {
                                        "m": [
                                            "CometExceptionDialog.react",
                                            "FDSTooltipDeferredImpl.react"
                                        ]
                                    },
                                    "rds": {
                                        "m": [
                                            "ContextualConfig",
                                            "BladeRunnerClient",
                                            "MAWMICSafe",
                                            "CometTabMenu.react",
                                            "FbtLogging",
                                            "DGWRequestStreamClient",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent",
                                            "CometRelayEF",
                                            "CometToast.react",
                                            "MqttLongPollingRunner"
                                        ],
                                        "r": [
                                            "BOv7jro",
                                            "7CxomUC",
                                            "AdpmZX+",
                                            "gxxmBEY",
                                            "mFOUf9V",
                                            "I9Os7/3"
                                        ]
                                    },
                                    "be": 1
                                },
                                "CometStickerPickerFlyoutTagSelectorRoot.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "UX5ZaR7",
                                        "q293ET7",
                                        "uLB6aZe",
                                        "eJ8EHGb",
                                        "gHB6UlN",
                                        "QHlvoYy",
                                        "tytAcfm"
                                    ],
                                    "rds": {
                                        "m": [
                                            "StickerStoreFalcoEvent",
                                            "CometSuspenseFalcoEvent"
                                        ],
                                        "r": [
                                            "f4wal+l"
                                        ]
                                    },
                                    "be": 1
                                },
                                "CometStickerPickerPopoverRoot.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "nhm6xwY",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "eJ8EHGb",
                                        "QHlvoYy"
                                    ],
                                    "be": 1
                                },
                                "CometStickerPickerStickerSearchCard.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "AdpmZX+",
                                        "AlP3gQE",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "UX5ZaR7",
                                        "Fo8wih0",
                                        "q293ET7",
                                        "uLB6aZe",
                                        "FC9h7XN",
                                        "eJ8EHGb",
                                        "8LWPrbs",
                                        "gHB6UlN",
                                        "QHlvoYy",
                                        "mbuNvlv",
                                        "tytAcfm"
                                    ],
                                    "rdfds": {
                                        "m": [
                                            "CometExceptionDialog.react",
                                            "FDSTooltipDeferredImpl.react"
                                        ]
                                    },
                                    "rds": {
                                        "m": [
                                            "ContextualConfig",
                                            "BladeRunnerClient",
                                            "FbtLogging",
                                            "StickerStoreFalcoEvent",
                                            "DGWRequestStreamClient",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent",
                                            "CometToast.react",
                                            "MAWMICSafe",
                                            "CometRelayEF",
                                            "MqttLongPollingRunner"
                                        ],
                                        "r": [
                                            "BOv7jro",
                                            "7CxomUC",
                                            "f4wal+l",
                                            "I9Os7/3",
                                            "mueC9mU"
                                        ]
                                    },
                                    "be": 1
                                },
                                "logStickersFlyoutHasOpened": {
                                    "r": [
                                        "v39gSxj",
                                        "f4wal+l",
                                        "vhKfY5c",
                                        "a/IJsf4"
                                    ],
                                    "be": 1
                                },
                                "CometTooltip_DEPRECATED.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "UX5ZaR7",
                                        "eJ8EHGb",
                                        "QHlvoYy",
                                        "uLB6aZe",
                                        "tytAcfm"
                                    ],
                                    "rdfds": {
                                        "m": [
                                            "CometTooltipDeferredImpl.react"
                                        ],
                                        "r": [
                                            "mbuNvlv"
                                        ]
                                    },
                                    "rds": {
                                        "m": [
                                            "CometSuspenseFalcoEvent",
                                            "FbtLogging",
                                            "IntlQtEventFalcoEvent"
                                        ]
                                    },
                                    "be": 1
                                },
                                "GroupsCometAnswerAgentEducationModal.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "+SU8cpz",
                                        "+uA+HvV",
                                        "AdpmZX+",
                                        "OjGdplo",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "7fNe6yM",
                                        "UX5ZaR7",
                                        "U952axk",
                                        "uLB6aZe",
                                        "Lx/GDfZ",
                                        "YBTqXQg",
                                        "eJ8EHGb",
                                        "QHlvoYy",
                                        "2hPt+8f",
                                        "mbuNvlv",
                                        "mueC9mU",
                                        "tytAcfm"
                                    ],
                                    "rdfds": {
                                        "m": [
                                            "CometExceptionDialog.react",
                                            "FDSTooltipDeferredImpl.react"
                                        ]
                                    },
                                    "rds": {
                                        "m": [
                                            "ContextualConfig",
                                            "BladeRunnerClient",
                                            "MAWMICSafe",
                                            "CometRelayEF",
                                            "FbtLogging",
                                            "DGWRequestStreamClient",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent",
                                            "CometToast.react",
                                            "MqttLongPollingRunner"
                                        ],
                                        "r": [
                                            "BOv7jro",
                                            "7CxomUC",
                                            "I9Os7/3"
                                        ]
                                    },
                                    "be": 1
                                },
                                "CometHovercardQueryRenderer.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "v39gSxj",
                                        "iHcJp2L",
                                        "cKZv3P8",
                                        "eJ8EHGb"
                                    ],
                                    "be": 1
                                },
                                "UserSignalsDetailsView.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "mv0ik3v",
                                        "UX5ZaR7",
                                        "YBTqXQg",
                                        "eJ8EHGb",
                                        "QHlvoYy",
                                        "mbuNvlv",
                                        "uLB6aZe"
                                    ],
                                    "rds": {
                                        "m": [
                                            "FbtLogging",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent"
                                        ]
                                    },
                                    "be": 1
                                },
                                "UserSignalsHovercard.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "AdpmZX+",
                                        "iLDhQqa",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "UX5ZaR7",
                                        "uLB6aZe",
                                        "ZDahxXw",
                                        "eJ8EHGb",
                                        "wBHmF39",
                                        "QHlvoYy",
                                        "2hPt+8f",
                                        "wyTDu/+",
                                        "mbuNvlv",
                                        "tytAcfm"
                                    ],
                                    "rdfds": {
                                        "m": [
                                            "CometTooltipDeferredImpl.react",
                                            "FDSTooltipDeferredImpl.react"
                                        ]
                                    },
                                    "rds": {
                                        "m": [
                                            "FbtLogging",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent",
                                            "UserSignalsClientClickEventFalcoEvent",
                                            "UserSignalsClientImpressionEventFalcoEvent"
                                        ],
                                        "r": [
                                            "3xZAcjl",
                                            "nVZGLFA"
                                        ]
                                    },
                                    "be": 1
                                },
                                "CometUFICodedErrorDialog.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "KrvVkDS",
                                        "UX5ZaR7",
                                        "uLB6aZe",
                                        "YBTqXQg",
                                        "eJ8EHGb",
                                        "QHlvoYy",
                                        "mbuNvlv",
                                        "tytAcfm"
                                    ],
                                    "rds": {
                                        "m": [
                                            "FbtLogging",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent"
                                        ]
                                    },
                                    "be": 1
                                },
                                "CometUFIShareActionLinkMenu.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "mbuNvlv",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "+kuUnwE",
                                        "/KCWsjQ",
                                        "cKZv3P8",
                                        "NFfKbD8",
                                        "UX5ZaR7",
                                        "uLB6aZe",
                                        "q3tcYA4",
                                        "Qac+fS7",
                                        "eJ8EHGb",
                                        "QHlvoYy",
                                        "bSfLrme",
                                        "tytAcfm"
                                    ],
                                    "rdfds": {
                                        "m": [
                                            "FDSTooltipDeferredImpl.react"
                                        ]
                                    },
                                    "rds": {
                                        "m": [
                                            "FbSharingEventFalcoEvent",
                                            "FbSharingSendFalcoEvent",
                                            "FbtLogging",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent"
                                        ],
                                        "r": [
                                            "ao/gvNJ"
                                        ]
                                    },
                                    "be": 1
                                },
                                "CometTextDelightAnimation.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "UX5ZaR7",
                                        "r5UmZvF",
                                        "uLB6aZe",
                                        "eJ8EHGb",
                                        "QHlvoYy",
                                        "tytAcfm"
                                    ],
                                    "rds": {
                                        "m": [
                                            "KeyframesRenderer",
                                            "FBKeyframesLoggedSession",
                                            "KeyframesAssetDecoder"
                                        ],
                                        "r": [
                                            "XogzSlm",
                                            "p6J0Y88",
                                            "BOv7jro",
                                            "7CxomUC"
                                        ]
                                    },
                                    "be": 1
                                },
                                "CometProfileVideoSection.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "92FWu0u",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "eJ8EHGb"
                                    ],
                                    "be": 1
                                },
                                "GroupsCometInviteOnMentionDialog.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "+uA+HvV",
                                        "AdpmZX+",
                                        "7iemgNg",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "UX5ZaR7",
                                        "uLB6aZe",
                                        "qZrkqYZ",
                                        "eJ8EHGb",
                                        "QHlvoYy",
                                        "2hPt+8f",
                                        "mbuNvlv",
                                        "mueC9mU",
                                        "tytAcfm"
                                    ],
                                    "rdfds": {
                                        "m": [
                                            "CometExceptionDialog.react",
                                            "FDSTooltipDeferredImpl.react"
                                        ]
                                    },
                                    "rds": {
                                        "m": [
                                            "ContextualConfig",
                                            "BladeRunnerClient",
                                            "CometToast.react",
                                            "MAWMICSafe",
                                            "FbtLogging",
                                            "DGWRequestStreamClient",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent",
                                            "CometRelayEF",
                                            "MqttLongPollingRunner"
                                        ],
                                        "r": [
                                            "BOv7jro",
                                            "7CxomUC",
                                            "I9Os7/3"
                                        ]
                                    },
                                    "be": 1
                                },
                                "Sticker.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "KpspYp1",
                                        "dPhs+py",
                                        "v39gSxj",
                                        "UX5ZaR7",
                                        "mo2I/T0",
                                        "uLB6aZe",
                                        "p8R/8l/",
                                        "eJ8EHGb",
                                        "2hPt+8f",
                                        "fxI9l/Y",
                                        "Yh/JWiF"
                                    ],
                                    "rds": {
                                        "m": [
                                            "FbtLogging",
                                            "IntlQtEventFalcoEvent"
                                        ]
                                    },
                                    "be": 1
                                },
                                "CometNewsRegulationDialog.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "SF5a4/N",
                                        "UX5ZaR7",
                                        "uLB6aZe",
                                        "X81AtpF",
                                        "YBTqXQg",
                                        "eJ8EHGb",
                                        "QHlvoYy",
                                        "mbuNvlv",
                                        "tytAcfm"
                                    ],
                                    "rdfds": {
                                        "m": [
                                            "FDSTooltipDeferredImpl.react"
                                        ]
                                    },
                                    "rds": {
                                        "m": [
                                            "FbtLogging",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent"
                                        ]
                                    },
                                    "be": 1
                                },
                                "SecuredActionBlockDialog.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "mbuNvlv",
                                        "XndYMPP",
                                        "wqwDtIe",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "UX5ZaR7",
                                        "TQMvJ5Y",
                                        "uLB6aZe",
                                        "n1/Vx7b",
                                        "ALBhwn6",
                                        "WpvFyQK",
                                        "oi7cBD/",
                                        "Qr223WB",
                                        "p8R/8l/",
                                        "X2lXaqk",
                                        "Qac+fS7",
                                        "eJ8EHGb",
                                        "QHlvoYy",
                                        "8sg2K08",
                                        "tytAcfm"
                                    ],
                                    "rds": {
                                        "m": [
                                            "CometToast.react",
                                            "MAWMICSafe",
                                            "FbtLogging",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent"
                                        ],
                                        "r": [
                                            "7CxomUC",
                                            "mueC9mU"
                                        ]
                                    },
                                    "be": 1
                                },
                                "SecuredActionChallengePasswordDialog.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "mbuNvlv",
                                        "2aWc0ax",
                                        "AdpmZX+",
                                        "AlP3gQE",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "Na1E3Dy",
                                        "UX5ZaR7",
                                        "CJ7ZV8+",
                                        "uLB6aZe",
                                        "YBTqXQg",
                                        "eJ8EHGb",
                                        "QHlvoYy",
                                        "2hPt+8f",
                                        "1eL6p1Q",
                                        "LtG+1uG",
                                        "mueC9mU",
                                        "tytAcfm"
                                    ],
                                    "rdfds": {
                                        "m": [
                                            "CometExceptionDialog.react",
                                            "FDSTooltipDeferredImpl.react"
                                        ]
                                    },
                                    "rds": {
                                        "m": [
                                            "ContextualConfig",
                                            "BladeRunnerClient",
                                            "MAWMICSafe",
                                            "FBBrowserPasswordEncryption",
                                            "FbtLogging",
                                            "DGWRequestStreamClient",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent",
                                            "CometToast.react",
                                            "CometRelayEF",
                                            "MqttLongPollingRunner"
                                        ],
                                        "r": [
                                            "BOv7jro",
                                            "7CxomUC",
                                            "I+GHswV",
                                            "R/kfhPG",
                                            "I9Os7/3"
                                        ]
                                    },
                                    "be": 1
                                },
                                "SecuredActionChallengeCDSPasswordDialog.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "mbuNvlv",
                                        "2aWc0ax",
                                        "XndYMPP",
                                        "AdpmZX+",
                                        "wqwDtIe",
                                        "AlP3gQE",
                                        "I+GHswV",
                                        "84Rk5n3",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "UX5ZaR7",
                                        "TQMvJ5Y",
                                        "uLB6aZe",
                                        "n1/Vx7b",
                                        "WpvFyQK",
                                        "oi7cBD/",
                                        "Qr223WB",
                                        "p8R/8l/",
                                        "LNCbLG/",
                                        "W+TDAGO",
                                        "X2lXaqk",
                                        "Qac+fS7",
                                        "eJ8EHGb",
                                        "QHlvoYy",
                                        "2hPt+8f",
                                        "mw2Kc1Z",
                                        "R/kfhPG",
                                        "8sg2K08",
                                        "tytAcfm"
                                    ],
                                    "rds": {
                                        "m": [
                                            "FbtLogging",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent"
                                        ]
                                    },
                                    "be": 1
                                },
                                "SecuredActionNoChallengeAvailableCDSDialog.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "mbuNvlv",
                                        "XndYMPP",
                                        "wqwDtIe",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "UX5ZaR7",
                                        "TQMvJ5Y",
                                        "uLB6aZe",
                                        "n1/Vx7b",
                                        "WpvFyQK",
                                        "oi7cBD/",
                                        "Qr223WB",
                                        "p8R/8l/",
                                        "LNCbLG/",
                                        "X2lXaqk",
                                        "Qac+fS7",
                                        "eJ8EHGb",
                                        "/NTWV2I",
                                        "QHlvoYy",
                                        "8sg2K08",
                                        "tytAcfm"
                                    ],
                                    "rds": {
                                        "m": [
                                            "FbtLogging",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent"
                                        ]
                                    },
                                    "be": 1
                                },
                                "TwoStepVerificationRoot.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "ZmGgkXA",
                                        "mbuNvlv",
                                        "2aWc0ax",
                                        "XndYMPP",
                                        "AdpmZX+",
                                        "wqwDtIe",
                                        "KKqBUon",
                                        "AlP3gQE",
                                        "6CoHJPY",
                                        "84Rk5n3",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "/KCWsjQ",
                                        "cKZv3P8",
                                        "7z1tgPR",
                                        "UX5ZaR7",
                                        "eNG9XyS",
                                        "jPMYVE1",
                                        "XnjZlAC",
                                        "TQMvJ5Y",
                                        "CMrhgpl",
                                        "uLB6aZe",
                                        "n1/Vx7b",
                                        "WpvFyQK",
                                        "oi7cBD/",
                                        "Qr223WB",
                                        "p8R/8l/",
                                        "gI8i2t+",
                                        "X2lXaqk",
                                        "Qac+fS7",
                                        "eJ8EHGb",
                                        "QHlvoYy",
                                        "2hPt+8f",
                                        "8sg2K08",
                                        "tytAcfm"
                                    ],
                                    "rdfds": {
                                        "m": [
                                            "CometExceptionDialog.react",
                                            "FDSTooltipDeferredImpl.react"
                                        ]
                                    },
                                    "rds": {
                                        "m": [
                                            "ContextualConfig",
                                            "BladeRunnerClient",
                                            "CometToast.react",
                                            "MAWMICSafe",
                                            "CometRelayEF",
                                            "FbtLogging",
                                            "DGWRequestStreamClient",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent",
                                            "MqttLongPollingRunner"
                                        ],
                                        "r": [
                                            "BOv7jro",
                                            "7CxomUC",
                                            "I9Os7/3",
                                            "mueC9mU"
                                        ]
                                    },
                                    "be": 1
                                },
                                "KeyframesRenderer": {
                                    "r": [
                                        "v39gSxj",
                                        "vhKfY5c",
                                        "XogzSlm"
                                    ],
                                    "be": 1
                                },
                                "FBKeyframesLoggedSession": {
                                    "r": [
                                        "p6J0Y88",
                                        "v39gSxj",
                                        "BOv7jro",
                                        "vhKfY5c",
                                        "uLB6aZe",
                                        "XogzSlm",
                                        "7CxomUC"
                                    ],
                                    "be": 1
                                },
                                "KeyframesAssetDecoder": {
                                    "r": [
                                        "p6J0Y88",
                                        "v39gSxj",
                                        "vhKfY5c",
                                        "uLB6aZe",
                                        "XogzSlm"
                                    ],
                                    "be": 1
                                },
                                "GroupsCometGroupRuleEntityDialog.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "tSjPifJ",
                                        "+uA+HvV",
                                        "AdpmZX+",
                                        "LpbHyFh",
                                        "RpwSNth",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "UX5ZaR7",
                                        "uLB6aZe",
                                        "YBTqXQg",
                                        "eJ8EHGb",
                                        "QHlvoYy",
                                        "2hPt+8f",
                                        "nlR+S3x",
                                        "Bw4pRwt",
                                        "mFOUf9V",
                                        "mbuNvlv",
                                        "mueC9mU",
                                        "Opz2BIO",
                                        "tytAcfm"
                                    ],
                                    "rdfds": {
                                        "m": [
                                            "CometExceptionDialog.react",
                                            "FDSTooltipDeferredImpl.react"
                                        ]
                                    },
                                    "rds": {
                                        "m": [
                                            "ContextualConfig",
                                            "BladeRunnerClient",
                                            "MAWMICSafe",
                                            "CometRelayEF",
                                            "FbtLogging",
                                            "GroupsViewedRulesFalcoEvent",
                                            "DGWRequestStreamClient",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent",
                                            "CometToast.react",
                                            "MqttLongPollingRunner"
                                        ],
                                        "r": [
                                            "BOv7jro",
                                            "7CxomUC",
                                            "I9Os7/3"
                                        ]
                                    },
                                    "be": 1
                                },
                                "KeyframesPluginRandomSubdocument": {
                                    "r": [
                                        "v39gSxj",
                                        "vhKfY5c",
                                        "mo2I/T0",
                                        "/b5dsuK"
                                    ],
                                    "be": 1
                                },
                                "KeyframesPluginRandomSubdocumentSchema": {
                                    "r": [
                                        "/b5dsuK"
                                    ],
                                    "be": 1
                                },
                                "KeyframesPluginSoundSchema": {
                                    "r": [
                                        "GfZQS3k",
                                        "XogzSlm"
                                    ],
                                    "be": 1
                                },
                                "KeyframesPluginSound": {
                                    "r": [
                                        "v39gSxj",
                                        "oCMPVVY",
                                        "XogzSlm",
                                        "vhKfY5c",
                                        "/b5dsuK"
                                    ],
                                    "be": 1
                                },
                                "KeyframesPluginTrimPathSchema": {
                                    "r": [
                                        "XogzSlm",
                                        "/b5dsuK"
                                    ],
                                    "be": 1
                                },
                                "KeyframesPluginTrimPath": {
                                    "r": [
                                        "v39gSxj",
                                        "vhKfY5c",
                                        "mFkoxEV",
                                        "XogzSlm",
                                        "/b5dsuK"
                                    ],
                                    "be": 1
                                },
                                "KeyframesPluginLayerNameSchema": {
                                    "r": [
                                        "A8Zmczg"
                                    ],
                                    "be": 1
                                },
                                "KeyframesPluginLayerName": {
                                    "r": [
                                        "eMxoRDZ",
                                        "/b5dsuK"
                                    ],
                                    "be": 1
                                },
                                "KeyframesPluginDynamicProperties": {
                                    "r": [
                                        "/b5dsuK",
                                        "inDZbxT"
                                    ],
                                    "be": 1
                                },
                                "KeyframesPluginDynamicPropertiesSchema": {
                                    "r": [
                                        "lqR6G6x"
                                    ],
                                    "be": 1
                                },
                                "KeyframesPluginLayerTags": {
                                    "r": [
                                        "v2p0ZYx",
                                        "/b5dsuK"
                                    ],
                                    "be": 1
                                },
                                "KeyframesPluginLayerTagsSchema": {
                                    "r": [
                                        "V0egoaT"
                                    ],
                                    "be": 1
                                },
                                "KeyframesPluginSubdocumentSwap": {
                                    "r": [
                                        "CMzu9iV",
                                        "/b5dsuK"
                                    ],
                                    "be": 1
                                },
                                "KeyframesPluginSubdocumentSwapSchema": {
                                    "r": [
                                        "qAifaaj"
                                    ],
                                    "be": 1
                                },
                                "CometProfileVerificationBadgePopover.react": {
                                    "r": [
                                        "vhKfY5c",
                                        "UZfqf8J",
                                        "v39gSxj",
                                        "cKZv3P8",
                                        "UX5ZaR7",
                                        "uLB6aZe",
                                        "eJ8EHGb",
                                        "jipJXH1",
                                        "QHlvoYy",
                                        "2hPt+8f",
                                        "tytAcfm"
                                    ],
                                    "rds": {
                                        "m": [
                                            "FbtLogging",
                                            "CometSuspenseFalcoEvent",
                                            "IntlQtEventFalcoEvent"
                                        ]
                                    },
                                    "be": 1
                                }
                            }
                        }
                    },
                    "jsmods": {
                        "define": [
                            [
                                "cr:6640",
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
                                "cr:619",
                                [
                                    "setTimeoutCometLoggingPriWWW"
                                ],
                                {
                                    "__rc": [
                                        "setTimeoutCometLoggingPriWWW",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:734",
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
                                "cr:755",
                                [
                                    "warningWWW"
                                ],
                                {
                                    "__rc": [
                                        "warningWWW",
                                        null
                                    ]
                                },
                                -1
                            ],
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
                                    "TimeSliceSham"
                                ],
                                {
                                    "__rc": [
                                        "TimeSliceSham",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:2874",
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
                                "cr:7063",
                                [
                                    "CometErrorBoundary.react"
                                ],
                                {
                                    "__rc": [
                                        "CometErrorBoundary.react",
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
                                "cr:7388",
                                [
                                    "setIntervalWWW"
                                ],
                                {
                                    "__rc": [
                                        "setIntervalWWW",
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
                                "cr:7422",
                                [
                                    "ImageDownloadTrackerWWW"
                                ],
                                {
                                    "__rc": [
                                        "ImageDownloadTrackerWWW",
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
                                "cr:8907",
                                [
                                    "HeroTracingCoreConfigWWW"
                                ],
                                {
                                    "__rc": [
                                        "HeroTracingCoreConfigWWW",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:8908",
                                [
                                    "HeroTracingCoreDependenciesWWW"
                                ],
                                {
                                    "__rc": [
                                        "HeroTracingCoreDependenciesWWW",
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
                                "cr:11054",
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
                                "cr:696703",
                                [
                                    "JSScheduler"
                                ],
                                {
                                    "__rc": [
                                        "JSScheduler",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:1080422",
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
                                "cr:1108857",
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
                                "cr:1294158",
                                [
                                    "React.classic"
                                ],
                                {
                                    "__rc": [
                                        "React.classic",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:1294159",
                                [
                                    "ReactDOM.classic"
                                ],
                                {
                                    "__rc": [
                                        "ReactDOM.classic",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:1522191",
                                [
                                    "CometLinkTrackingUtils.facebook"
                                ],
                                {
                                    "__rc": [
                                        "CometLinkTrackingUtils.facebook",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:70",
                                [
                                    "FBInteractionTracingDependencies"
                                ],
                                {
                                    "__rc": [
                                        "FBInteractionTracingDependencies",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:686",
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
                                "cr:873",
                                [
                                    "InteractionTracing"
                                ],
                                {
                                    "__rc": [
                                        "InteractionTracing",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:2448",
                                [
                                    "useHeroBootloadedComponent"
                                ],
                                {
                                    "__rc": [
                                        "useHeroBootloadedComponent",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:4874",
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
                                "cr:7383",
                                [
                                    "BanzaiWWW"
                                ],
                                {
                                    "__rc": [
                                        "BanzaiWWW",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:7451",
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
                                "cr:8546",
                                [
                                    "FDSCometTooltip.react"
                                ],
                                {
                                    "__rc": [
                                        "FDSCometTooltip.react",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:719780",
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
                                "cr:955714",
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
                                "cr:1011783",
                                [
                                    "CometHeroInteractionImpl.react"
                                ],
                                {
                                    "__rc": [
                                        "CometHeroInteractionImpl.react",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:1064332",
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
                                "cr:1106516",
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
                                "cr:1645510",
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
                                "cr:1752405",
                                [
                                    "QPLAddCometRequestHeaders"
                                ],
                                {
                                    "__rc": [
                                        "QPLAddCometRequestHeaders",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:1802022",
                                [
                                    "CometPrerenderer.react"
                                ],
                                {
                                    "__rc": [
                                        "CometPrerenderer.react",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:1802023",
                                [
                                    "BaseContextualLayerDefaultContainer.react"
                                ],
                                {
                                    "__rc": [
                                        "BaseContextualLayerDefaultContainer.react",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:1941981",
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
                                "cr:1941982",
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
                                "cr:1984081",
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
                                "cr:2010754",
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
                                "cr:370",
                                [
                                    "Lexical.prod"
                                ],
                                {
                                    "__rc": [
                                        "Lexical.prod",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:267",
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
                                "cr:641",
                                [
                                    "handleCometErrorCodeSideEffects"
                                ],
                                {
                                    "__rc": [
                                        "handleCometErrorCodeSideEffects",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:851",
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
                                "cr:984",
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
                                "cr:1196",
                                [
                                    "handleCometReauthenticationSideEffects"
                                ],
                                {
                                    "__rc": [
                                        "handleCometReauthenticationSideEffects",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:2701",
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
                                "cr:5655",
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
                                "cr:7299",
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
                                "cr:7438",
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
                                    "RunComet"
                                ],
                                {
                                    "__rc": [
                                        "RunComet",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:1110430",
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
                                "cr:1121434",
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
                                "cr:1467370",
                                [
                                    "CometRelayScheduler"
                                ],
                                {
                                    "__rc": [
                                        "CometRelayScheduler",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:2181",
                                [
                                    "LexicalText.prod"
                                ],
                                {
                                    "__rc": [
                                        "LexicalText.prod",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:509",
                                [
                                    "LexicalComposerContext.prod"
                                ],
                                {
                                    "__rc": [
                                        "LexicalComposerContext.prod",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:2099",
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
                                "cr:273",
                                [
                                    "FocusWithinHandlerNonStrictMode_DEPRECATED.react"
                                ],
                                {
                                    "__rc": [
                                        "FocusWithinHandlerNonStrictMode_DEPRECATED.react",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:6669",
                                [
                                    "DataStore"
                                ],
                                {
                                    "__rc": [
                                        "DataStore",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:1752989",
                                [
                                    "CometAnimatedReactionIcon.react"
                                ],
                                {
                                    "__rc": [
                                        "CometAnimatedReactionIcon.react",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:1752990",
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
                                "cr:2011405",
                                [
                                    "CometDefaultKeyCommands"
                                ],
                                {
                                    "__rc": [
                                        "CometDefaultKeyCommands",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:2011406",
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
                                "cr:244",
                                [
                                    "CometEmoji.react"
                                ],
                                {
                                    "__rc": [
                                        "CometEmoji.react",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:945",
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
                                "cr:2169",
                                [
                                    "URITruncator"
                                ],
                                {
                                    "__rc": [
                                        "URITruncator",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:3118",
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
                                "cr:3119",
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
                                "cr:3258",
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
                                "cr:3749",
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
                                "cr:6699",
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
                                "cr:6969",
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
                                "cr:994756",
                                [
                                    "BaseCometModal.react"
                                ],
                                {
                                    "__rc": [
                                        "BaseCometModal.react",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:1691800",
                                [
                                    "CometLinkedEntityRenderer"
                                ],
                                {
                                    "__rc": [
                                        "CometLinkedEntityRenderer",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:1824473",
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
                                "CometPersistQueryParams",
                                [],
                                {
                                    "relative": {},
                                    "domain": {}
                                },
                                6231
                            ],
                            [
                                "IntlVariationHoldout",
                                [],
                                {
                                    "disable_variation": false
                                },
                                6533
                            ],
                            [
                                "ClickIDURLBlocklistSVConfig",
                                [],
                                {
                                    "block_list_url": [
                                        ""
                                    ]
                                },
                                7631
                            ],
                            [
                                "BootloaderConfig",
                                [],
                                {
                                    "deferBootloads": false,
                                    "jsRetries": [
                                        200,
                                        500
                                    ],
                                    "jsRetryAbortNum": 2,
                                    "jsRetryAbortTime": 5,
                                    "silentDups": true,
                                    "timeout": 60000,
                                    "tieredLoadingFromTier": 100,
                                    "hypStep4": true,
                                    "phdOn": true,
                                    "btCutoffIndex": 6586,
                                    "fastPathForAlreadyRequired": true,
                                    "earlyRequireLazy": false,
                                    "enableTimeoutLoggingForNonComet": true,
                                    "deferLongTailManifest": true,
                                    "lazySoT": false,
                                    "translationRetries": [
                                        200,
                                        500
                                    ],
                                    "translationRetryAbortNum": 3,
                                    "translationRetryAbortTime": 50
                                },
                                329
                            ],
                            [
                                "CSSLoaderConfig",
                                [],
                                {
                                    "timeout": 5000,
                                    "modulePrefix": "BLCSS:",
                                    "forcePollForBootloader": true,
                                    "loadEventSupported": true
                                },
                                619
                            ],
                            [
                                "IntlPhonologicalRules",
                                [],
                                {
                                    "meta": {},
                                    "patterns": {}
                                },
                                1496
                            ],
                            [
                                "IntlViewerContext",
                                [],
                                {
                                    "GENDER": 1,
                                    "regionalLocale": null
                                },
                                772
                            ],
                            [
                                "LSD",
                                [],
                                {
                                    "token": "0WAinO5gR6h9tZVv5Mwoo3"
                                },
                                323
                            ],
                            [
                                "NumberFormatConfig",
                                [],
                                {
                                    "decimalSeparator": ",",
                                    "numberDelimiter": ".",
                                    "minDigitsForThousandsSeparator": 4,
                                    "standardDecimalPatternInfo": {
                                        "primaryGroupSize": 3,
                                        "secondaryGroupSize": 3
                                    },
                                    "numberingSystemData": null
                                },
                                54
                            ],
                            [
                                "RelayAPIConfigDefaults",
                                [],
                                {
                                    "accessToken": "",
                                    "actorID": "61557504676830",
                                    "customHeaders": {},
                                    "enableNetworkLogger": false,
                                    "fetchTimeout": 30000,
                                    "graphBatchURI": "/api/graphqlbatch/",
                                    "graphURI": "/api/graphql/",
                                    "retryDelays": [
                                        1000,
                                        3000
                                    ],
                                    "useXController": true,
                                    "xhrEncoding": null,
                                    "subscriptionTopicURI": null,
                                    "withCredentials": false,
                                    "isProductionEndpoint": false,
                                    "workRequestTaggingProduct": null,
                                    "encryptionKeyParams": null
                                },
                                926
                            ],
                            [
                                "ServerNonce",
                                [],
                                {
                                    "ServerNonce": "-V-xj1PEDhiC6yl7lDVM6q"
                                },
                                141
                            ],
                            [
                                "SiteData",
                                [],
                                {
                                    "server_revision": 1012776817,
                                    "client_revision": 1012776817,
                                    "push_phase": "C3",
                                    "pkg_cohort": "HYP:comet_pkg",
                                    "haste_session": "19828.HYP:comet_pkg.2.1..2.1",
                                    "pr": 1.5,
                                    "manifest_base_uri": "https://static.xx.fbcdn.net",
                                    "manifest_origin": "facebook",
                                    "manifest_version_prefix": "",
                                    "be_one_ahead": true,
                                    "is_rtl": false,
                                    "is_experimental_tier": false,
                                    "is_jit_warmed_up": true,
                                    "hsi": "7358014083303114264",
                                    "semr_host_bucket": "3",
                                    "bl_hash_version": 2,
                                    "comet_env": 15,
                                    "wbloks_env": false,
                                    "ef_page": "relay_ef:CommentListComponentsRootQuery",
                                    "compose_bootloads": false,
                                    "spin": 4,
                                    "__spin_r": 1012776817,
                                    "__spin_b": "trunk",
                                    "__spin_t": 1713171160,
                                    "vip": "163.70.159.35"
                                },
                                317
                            ],
                            [
                                "SprinkleConfig",
                                [],
                                {
                                    "param_name": "jazoest",
                                    "version": 2,
                                    "should_randomize": false
                                },
                                2111
                            ],
                            [
                                "UserAgentData",
                                [],
                                {
                                    "browserArchitecture": "32",
                                    "browserFullVersion": "61.0",
                                    "browserMinorVersion": 0,
                                    "browserName": "Firefox",
                                    "browserVersion": 61,
                                    "deviceName": "Unknown",
                                    "engineName": "Blink",
                                    "engineVersion": "119.0.6045.200",
                                    "platformArchitecture": "32",
                                    "platformName": "Windows",
                                    "platformVersion": "Vista",
                                    "platformFullVersion": "Vista"
                                },
                                527
                            ],
                            [
                                "PromiseUsePolyfillSetImmediateGK",
                                [],
                                {
                                    "www_always_use_polyfill_setimmediate": false
                                },
                                2190
                            ],
                            [
                                "KSConfig",
                                [],
                                {
                                    "killed": {
                                        "__set": [
                                            "POCKET_MONSTERS_CREATE",
                                            "POCKET_MONSTERS_DELETE",
                                            "POCKET_MONSTERS_UPDATE_NAME",
                                            "TPA_SRT_TRANSLATION",
                                            "WORKROOMS_REQUEST_TAGGING_TAG_NO_INIT_BY_VC_GALAXY"
                                        ]
                                    },
                                    "ko": {
                                        "__set": [
                                            "acrJTh9WGdp",
                                            "1oOE64fL4wO",
                                            "7r6mSP7ofr2",
                                            "3sKizTQ6byg",
                                            "6XsXQ2qHw8y"
                                        ]
                                    }
                                },
                                2580
                            ],
                            [
                                "JSErrorLoggingConfig",
                                [],
                                {
                                    "appId": 2220391788200892,
                                    "extra": [],
                                    "reportInterval": 50,
                                    "sampleWeight": null,
                                    "sampleWeightKey": "__jssesw",
                                    "projectBlocklist": []
                                },
                                2776
                            ],
                            [
                                "ImmediateImplementationExperiments",
                                [],
                                {
                                    "prefer_message_channel": true
                                },
                                3419
                            ],
                            [
                                "FBDomainsSVConfig",
                                [],
                                {
                                    "domains": {
                                        "__map": [
                                            [
                                                "www.facebook.com",
                                                1
                                            ],
                                            [
                                                "tfbnw.net",
                                                1
                                            ],
                                            [
                                                "m.beta.facebook.com",
                                                1
                                            ],
                                            [
                                                "touch.beta.facebook.com",
                                                1
                                            ],
                                            [
                                                "www.dev.facebook.com",
                                                1
                                            ],
                                            [
                                                "fb.me",
                                                1
                                            ],
                                            [
                                                "s.fb.com",
                                                1
                                            ],
                                            [
                                                "m.fbjs.facebook.com",
                                                1
                                            ],
                                            [
                                                "facebook.com.es",
                                                1
                                            ],
                                            [
                                                "www.fbjs.facebook.com",
                                                1
                                            ],
                                            [
                                                "m.facebook.com",
                                                1
                                            ],
                                            [
                                                "facebook.fr",
                                                1
                                            ],
                                            [
                                                "fbsbx.com",
                                                1
                                            ],
                                            [
                                                "embed.fbsbx.com",
                                                1
                                            ],
                                            [
                                                "attachment.fbsbx.com",
                                                1
                                            ],
                                            [
                                                "lookaside.fbsbx.com",
                                                1
                                            ],
                                            [
                                                "web.facebook.com",
                                                1
                                            ],
                                            [
                                                "fb.com",
                                                1
                                            ],
                                            [
                                                "messenger.com",
                                                1
                                            ],
                                            [
                                                "secure.facebook.com",
                                                1
                                            ],
                                            [
                                                "secure.my-od.facebook.com",
                                                1
                                            ],
                                            [
                                                "www.my-od.facebook.com",
                                                1
                                            ]
                                        ]
                                    }
                                },
                                3828
                            ],
                            [
                                "ClickIDDomainBlacklistSVConfig",
                                [],
                                {
                                    "domains": [
                                        "craigslist",
                                        "tfbnw.net",
                                        "flashtalking.com",
                                        "canadiantire.ca",
                                        "o2.co.uk",
                                        "archive.org",
                                        "reddit.com",
                                        "redd.it",
                                        "gmail.com",
                                        "cvk.gov.ua",
                                        "electoralsearch.in",
                                        "yahoo.com",
                                        "cve.mitre.org",
                                        "usenix.org",
                                        "ky.gov",
                                        "voteohio.gov",
                                        "vote.pa.gov",
                                        "oversightboard.com",
                                        "wi.gov",
                                        "pbs.twimg.com",
                                        "media.discordapp.net",
                                        "vastadeal.com",
                                        "theaustralian.com.au",
                                        "alloygator.com",
                                        "elsmannimmobilien.de",
                                        "news.com.au",
                                        "dennisbonnen.com",
                                        "stoett.com",
                                        "investorhour.com",
                                        "perspectivasur.com",
                                        "bonnegueule.fr",
                                        "firstent.org",
                                        "twitpic.com",
                                        "kollosche.com.au",
                                        "nau.edu",
                                        "arcourts.gov",
                                        "lomberg.de",
                                        "network4.hu",
                                        "balloonrace.com",
                                        "awstrack.me",
                                        "ic3.gov",
                                        "sos.wyo.gov",
                                        "cnpq.br",
                                        "0.discoverapp.com",
                                        "apple.com",
                                        "apple.co",
                                        "applecard.apple",
                                        "services.apple",
                                        "appletvplus.com",
                                        "applepay.apple",
                                        "beatsbydre.com",
                                        "dinn.com.mx",
                                        "soriana.com",
                                        "facebook.sso.datasite.com",
                                        "fycextras.com",
                                        "rik.parlament.gov.rs",
                                        "dge.sn"
                                    ]
                                },
                                3829
                            ],
                            [
                                "UriNeedRawQuerySVConfig",
                                [],
                                {
                                    "uris": [
                                        "dms.netmng.com",
                                        "doubleclick.net",
                                        "r.msn.com",
                                        "watchit.sky.com",
                                        "graphite.instagram.com",
                                        "www.kfc.co.th",
                                        "learn.pantheon.io",
                                        "www.landmarkshops.in",
                                        "www.ncl.com",
                                        "s0.wp.com",
                                        "www.tatacliq.com",
                                        "bs.serving-sys.com",
                                        "kohls.com",
                                        "lazada.co.th",
                                        "xg4ken.com",
                                        "technopark.ru",
                                        "officedepot.com.mx",
                                        "bestbuy.com.mx",
                                        "booking.com",
                                        "nibio.no",
                                        "myworkdayjobs.com",
                                        "united-united.com"
                                    ]
                                },
                                3871
                            ],
                            [
                                "InitialCookieConsent",
                                [],
                                {
                                    "deferCookies": false,
                                    "initialConsent": [
                                        1,
                                        2
                                    ],
                                    "noCookies": false,
                                    "shouldShowCookieBanner": false,
                                    "shouldWaitForDeferredDatrCookie": false
                                },
                                4328
                            ],
                            [
                                "WebConnectionClassServerGuess",
                                [],
                                {
                                    "connectionClass": "EXCELLENT"
                                },
                                4705
                            ],
                            [
                                "BootloaderEndpointConfig",
                                [],
                                {
                                    "debugNoBatching": false,
                                    "maxBatchSize": -1,
                                    "endpointURI": "https://www.facebook.com/ajax/bootloader-endpoint/"
                                },
                                5094
                            ],
                            [
                                "CookieConsentIFrameConfig",
                                [],
                                {
                                    "consent_param": "FQARERESAA==.ARb0pDNXOfS1UaYgneNGRtoZyGn2knURKVB8y4l1c9JvAlDk",
                                    "allowlisted_iframes": [],
                                    "is_checkpointed": false
                                },
                                5540
                            ],
                            [
                                "ServerTimeData",
                                [],
                                {
                                    "serverTime": 1713171160692,
                                    "timeOfRequestStart": 1713171160442.4,
                                    "timeOfResponseStart": 1713171160442.4
                                },
                                5943
                            ],
                            [
                                "IntlCurrentLocale",
                                [],
                                {
                                    "code": "vi_VN"
                                },
                                5954
                            ],
                            [
                                "CookieDomain",
                                [],
                                {
                                    "domain": "facebook.com"
                                },
                                6421
                            ],
                            [
                                "JSSelfProfilerTrackedInteractions",
                                [],
                                {
                                    "interactions": [
                                        {
                                            "action": "*",
                                            "tracePolicy": "*"
                                        }
                                    ]
                                },
                                6918
                            ],
                            [
                                "CookieCoreConfig",
                                [],
                                {
                                    "c_user": {
                                        "t": 31536000
                                    },
                                    "cppo": {
                                        "t": 86400
                                    },
                                    "dpr": {
                                        "t": 604800
                                    },
                                    "fbl_ci": {
                                        "t": 31536000
                                    },
                                    "fbl_cs": {
                                        "t": 31536000
                                    },
                                    "fbl_st": {
                                        "t": 31536000
                                    },
                                    "i_user": {
                                        "t": 31536000
                                    },
                                    "locale": {
                                        "t": 604800
                                    },
                                    "m_ls": {
                                        "t": 34560000
                                    },
                                    "m_pixel_ratio": {
                                        "t": 604800
                                    },
                                    "noscript": {},
                                    "presence": {
                                        "t": 2592000
                                    },
                                    "sfau": {},
                                    "usida": {},
                                    "vpd": {
                                        "t": 5184000
                                    },
                                    "wd": {
                                        "t": 604800
                                    },
                                    "wl_cbv": {
                                        "t": 7776000
                                    },
                                    "x-referer": {},
                                    "x-src": {
                                        "t": 1
                                    }
                                },
                                2104
                            ],
                            [
                                "CookieCoreLoggingConfig",
                                [],
                                {
                                    "maximumIgnorableStallMs": 16.67,
                                    "sampleRate": 9.7E-05,
                                    "sampleRateClassic": 1E-10,
                                    "sampleRateFastStale": 1E-08
                                },
                                3401
                            ],
                            [
                                "USIDMetadata",
                                [],
                                {
                                    "browser_id": "?",
                                    "tab_id": "",
                                    "page_id": "Psbz7bsdir9hf",
                                    "transition_id": 0,
                                    "version": 6
                                },
                                5888
                            ],
                            [
                                "UFICommentFileInputAcceptValues",
                                [],
                                {
                                    "both": "video/*,  video/x-m4v, video/webm, video/x-ms-wmv, video/x-msvideo, video/3gpp, video/flv, video/x-flv, video/mp4, video/quicktime, video/mpeg, video/ogv, .ts, .mkv, image/*, image/heic, image/heif",
                                    "photos": "image/*, image/heic, image/heif",
                                    "videos": "video/*, video/x-m4v, video/webm, video/x-ms-wmv, video/x-msvideo, video/3gpp, video/flv, video/x-flv, video/mp4, video/quicktime, video/mpeg, video/ogv, .ts, .mkv",
                                    "files": "application/*, application/pdf, application/x-pdf, application/x-bzpdf, application/x-gzpdf, application/msword, application/vnd.openxmlformats-officedocument.wordprocessingml.document, application/vnd.ms-powerpoint, application/vnd.openxmlformats-officedocument.presentationml.presentation, application/vnd.openxmlformats-officedocument.spreadsheetml.sheet, application/vnd.ms-excel, text/*, image/*, image/heic, image/heif, model/*, video/*, video/x-m4v, video/webm, video/x-ms-wmv, video/x-msvideo, video/3gpp, video/flv, video/x-flv, video/mp4, video/quicktime, video/mpeg, video/ogv, .ts, .mkv"
                                },
                                1317
                            ],
                            [
                                "TransportSelectingClientContextualConfig",
                                [],
                                {
                                    "rawConfig": "{\"name\":\"rti/web_rs_transport_selecting_client\",\"cctype\":\"dense\",\"version\":1,\"policy_id\":\"static\",\"sample_rate\":1000,\"contexts\":[{\"name\":\"method\",\"type\":\"STRING\",\"callsite\":true,\"buckets\":[{\"name\":\"rollout_group_1\",\"strategy\":\"in\",\"values\":[\"FBGQLS:FEEDBACK_LIKE_SUBSCRIBE\",\"Falco\",\"FBLQ:comet_notifications_live_query_experimental\"]},{\"name\":\"rollout_group_6\",\"strategy\":\"in\",\"values\":[\"FBGQLS:COMMENT_CREATE_SUBSCRIBE\",\"FBGQLS:COMMENT_LIKE_SUBSCRIBE\",\"FBGQLS:FEEDBACK_COMMENT_PERMISSION_TOGGLE_SUBSCRIBE\",\"FBGQLS:FEEDBACK_TYPING_SUBSCRIBE\"]},{\"name\":\"rollout_group_4\",\"strategy\":\"regex\",\"values\":[\"FBGQLS:.*\"]},{\"name\":\"rollout_group_3\",\"strategy\":\"regex\",\"values\":[\"FBLQ:.*\"]},{\"name\":\"skywalker\",\"strategy\":\"in\",\"values\":[\"SKY:test_topic\",\"live/api/copyright\",\"intern_notify\",\"locplat/ttm\",\"rti_widget_dashboard\",\"srt/user_metrics_counter\",\"media_manager_instagram_composer_create_update\",\"cubism_annotations/fleet_health\",\"srt/notifications\",\"ads/reporting/snapshot\",\"unidash/widget\",\"cubism_annotations\",\"ads/reporting/export\",\"pubx/notification/update\",\"ads/powereditor/import\",\"lwi_async_create\",\"video_edit\",\"metric_graph_realtime\",\"vcc_video_posting_www\",\"cms/object_archive_copy_created\",\"cms/branch_updated\",\"cms/object_saved\",\"codeless_event_tracking\",\"srt/job_updated\",\"video_broadcast\",\"video/broadcast/error\",\"vcpanel/api\",\"lwi_everywhere_plugin\",\"commercial_break_v2\",\"advanced_analytics/query\",\"cubism_annotations/ads_mastercook_models\",\"gqls/comment_like_subscribe\",\"live/api/copyright\",\"shiba/mock_bot_error\",\"shiba/save_state\",\"video_list_publishing_progress_update\",\"assistant_wizard\",\"gizmo/manage\",\"collab/presentation/request\",\"snaptu/push_notif\"]},{\"name\":\"skywalker_bulletin\",\"strategy\":\"in\",\"values\":[\"www/sr/hot_reload\"]},{\"name\":\"rollout_group_5\",\"strategy\":\"regex\",\"values\":[\"Collabri|RealtimeClientSync:.*\"]},{\"name\":\"default\",\"strategy\":\"catch_all\"}]}],\"outputs\":[{\"name\":\"group\",\"type\":\"STRING\"},{\"name\":\"dgwUpsampleMultiplier\",\"type\":\"FLOAT\"}],\"vector\":[\"group1\",\"0.01\",\"group6\",\"0.001\",\"group4\",\"1.0\",\"group3\",\"1.0\",\"skywalker\",\"1.0\",\"skywalker_bulletin\",\"1.0\",\"group5\",\"1.0\",\"default_group\",\"1.0\"],\"vectorDefaults\":[\"default_group\",\"1.0\"],\"timestamp\":1663366072}"
                                },
                                5968
                            ],
                            [
                                "RtiWebRequestStreamClient",
                                [],
                                {
                                    "ThrottledMethods": {},
                                    "overrideHeaders": {}
                                },
                                6639
                            ],
                            [
                                "ZeroCategoryHeader",
                                [],
                                {},
                                1127
                            ],
                            [
                                "ZeroRewriteRules",
                                [],
                                {
                                    "rewrite_rules": {},
                                    "whitelist": {
                                        "/hr/r": 1,
                                        "/hr/p": 1,
                                        "/zero/unsupported_browser/": 1,
                                        "/zero/policy/optin": 1,
                                        "/zero/optin/write/": 1,
                                        "/zero/optin/legal/": 1,
                                        "/zero/optin/free/": 1,
                                        "/about/privacy/": 1,
                                        "/about/privacy/update/": 1,
                                        "/privacy/explanation/": 1,
                                        "/zero/toggle/welcome/": 1,
                                        "/zero/toggle/nux/": 1,
                                        "/zero/toggle/settings/": 1,
                                        "/fup/interstitial/": 1,
                                        "/work/landing": 1,
                                        "/work/login/": 1,
                                        "/work/email/": 1,
                                        "/ai.php": 1,
                                        "/js_dialog_resources/dialog_descriptions_android.json": 0,
                                        "/connect/jsdialog/MPlatformAppInvitesJSDialog/": 0,
                                        "/connect/jsdialog/MPlatformOAuthShimJSDialog/": 0,
                                        "/connect/jsdialog/MPlatformLikeJSDialog/": 0,
                                        "/qp/interstitial/": 1,
                                        "/qp/action/redirect/": 1,
                                        "/qp/action/close/": 1,
                                        "/zero/support/ineligible/": 1,
                                        "/zero_balance_redirect/": 1,
                                        "/zero_balance_redirect": 1,
                                        "/zero_balance_redirect/l/": 1,
                                        "/l.php": 1,
                                        "/lsr.php": 1,
                                        "/ajax/dtsg/": 1,
                                        "/checkpoint/block/": 1,
                                        "/exitdsite": 1,
                                        "/zero/balance/pixel/": 1,
                                        "/zero/balance/": 1,
                                        "/zero/balance/carrier_landing/": 1,
                                        "/zero/flex/logging/": 1,
                                        "/tr": 1,
                                        "/tr/": 1,
                                        "/sem_campaigns/sem_pixel_test/": 1,
                                        "/bookmarks/flyout/body/": 1,
                                        "/zero/subno/": 1,
                                        "/confirmemail.php": 1,
                                        "/policies/": 1,
                                        "/mobile/internetdotorg/classifier/": 1,
                                        "/zero/dogfooding": 1,
                                        "/xti.php": 1,
                                        "/zero/fblite/config/": 1,
                                        "/hr/zsh/wc/": 1,
                                        "/ajax/bootloader-endpoint/": 1,
                                        "/mobile/zero/carrier_page/": 1,
                                        "/mobile/zero/carrier_page/education_page/": 1,
                                        "/mobile/zero/carrier_page/feature_switch/": 1,
                                        "/mobile/zero/carrier_page/settings_page/": 1,
                                        "/aloha_check_build": 1,
                                        "/upsell/zbd/softnudge/": 1,
                                        "/mobile/zero/af_transition/": 1,
                                        "/mobile/zero/af_transition/action/": 1,
                                        "/mobile/zero/freemium/": 1,
                                        "/mobile/zero/freemium/redirect/": 1,
                                        "/mobile/zero/freemium/zero_fup/": 1,
                                        "/privacy/policy/": 1,
                                        "/privacy/center/": 1,
                                        "/data/manifest/": 1,
                                        "/4oh4.php": 1,
                                        "/autologin.php": 1,
                                        "/birthday_help.php": 1,
                                        "/checkpoint/": 1,
                                        "/contact-importer/": 1,
                                        "/cr.php": 1,
                                        "/legal/terms/": 1,
                                        "/login.php": 1,
                                        "/login/": 1,
                                        "/mobile/account/": 1,
                                        "/n/": 1,
                                        "/remote_test_device/": 1,
                                        "/upsell/buy/": 1,
                                        "/upsell/buyconfirm/": 1,
                                        "/upsell/buyresult/": 1,
                                        "/upsell/promos/": 1,
                                        "/upsell/continue/": 1,
                                        "/upsell/h/promos/": 1,
                                        "/upsell/loan/learnmore/": 1,
                                        "/upsell/purchase/": 1,
                                        "/upsell/promos/upgrade/": 1,
                                        "/upsell/buy_redirect/": 1,
                                        "/upsell/loan/buyconfirm/": 1,
                                        "/upsell/loan/buy/": 1,
                                        "/upsell/sms/": 1,
                                        "/wap/a/channel/reconnect.php": 1,
                                        "/wap/a/nux/wizard/nav.php": 1,
                                        "/wap/appreg.php": 1,
                                        "/wap/birthday_help.php": 1,
                                        "/wap/c.php": 1,
                                        "/wap/confirmemail.php": 1,
                                        "/wap/cr.php": 1,
                                        "/wap/login.php": 1,
                                        "/wap/r.php": 1,
                                        "/zero/datapolicy": 1,
                                        "/a/timezone.php": 1,
                                        "/a/bz": 1,
                                        "/bz/reliability": 1,
                                        "/r.php": 1,
                                        "/mr/": 1,
                                        "/reg/": 1,
                                        "/registration/log/": 1,
                                        "/terms/": 1,
                                        "/f123/": 1,
                                        "/expert/": 1,
                                        "/experts/": 1,
                                        "/terms/index.php": 1,
                                        "/terms.php": 1,
                                        "/srr/": 1,
                                        "/msite/redirect/": 1,
                                        "/fbs/pixel/": 1,
                                        "/contactpoint/preconfirmation/": 1,
                                        "/contactpoint/cliff/": 1,
                                        "/contactpoint/confirm/submit/": 1,
                                        "/contactpoint/confirmed/": 1,
                                        "/contactpoint/login/": 1,
                                        "/preconfirmation/contactpoint_change/": 1,
                                        "/help/contact/": 1,
                                        "/survey/": 1,
                                        "/upsell/loyaltytopup/accept/": 1,
                                        "/settings/": 1,
                                        "/lite/": 1,
                                        "/zero_status_update/": 1,
                                        "/operator_store/": 1,
                                        "/upsell/": 1,
                                        "/wifiauth/login/": 1
                                    }
                                },
                                1478
                            ],
                            [
                                "CometRelayConfig",
                                [],
                                {
                                    "gc_release_buffer_size": 50
                                },
                                4685
                            ],
                            [
                                "MqttWebDeviceID",
                                [],
                                {
                                    "clientID": "442352a8-23c6-4cc6-b432-dd19f3bad0ab"
                                },
                                5003
                            ],
                            [
                                "LiveQueryWebRelayKillList",
                                [],
                                {
                                    "liveQueryWebRelayKillList": [
                                        "test_example_config_id_to_be_killed",
                                        "data_studio_nav_pane_collections_section",
                                        "work_recruiting_home_tasks"
                                    ]
                                },
                                5050
                            ],
                            [
                                "LiveQueryWebClientPollingSwitchList",
                                [],
                                {
                                    "liveQueryWebClientPollingSwitchList": {
                                        "example_config_id_to_be_switched": 10000
                                    }
                                },
                                5842
                            ],
                            [
                                "CLDRDateFormatConfig",
                                [],
                                {
                                    "supportedPHPFormatsKeys": {
                                        "D": "E",
                                        "D g:ia": "Ejm",
                                        "D M d": "MMMEd",
                                        "D M d, Y": "yMMMEd",
                                        "D M j": "MMMEd",
                                        "D M j, y": "yMMMEd",
                                        "D, M j": "MMMEd",
                                        "D, M j, Y": "yMMMEd",
                                        "F d": "MMMMd",
                                        "F d, Y": "date_long",
                                        "F j": "MMMMd",
                                        "F j, Y": "date_long",
                                        "F j, Y @ g:i A": "dateTime_long_short",
                                        "F j, Y g:i a": "dateTime_long_short",
                                        "F j, Y @ g:i:s A": "dateTime_long_medium",
                                        "F jS": "MMMMd",
                                        "F jS, g:ia": "dateTime_long_short",
                                        "F jS, Y": "date_long",
                                        "F Y": "yMMMM",
                                        "g A": "j",
                                        "G:i": "time_short",
                                        "g:i": "time_short",
                                        "g:i a": "time_short",
                                        "g:i A": "time_short",
                                        "g:i:s A": "time_medium",
                                        "g:ia": "time_short",
                                        "g:iA": "time_short",
                                        "g:ia F jS, Y": "dateTime_long_short",
                                        "g:iA l, F jS": "dateTime_full_short",
                                        "g:ia M jS": "dateTime_medium_short",
                                        "g:ia, F jS": "dateTime_long_short",
                                        "g:iA, l M jS": "dateTime_full_short",
                                        "h:i a": "time_short",
                                        "h:m:s m/d/Y": "dateTime_short_short",
                                        "j": "d",
                                        "j F Y": "date_long",
                                        "l F d, Y": "date_full",
                                        "l, F d, Y": "date_full",
                                        "l, F j": "date_full",
                                        "l, F j, Y": "date_full",
                                        "l, F jS": "date_full",
                                        "l, F jS, g:ia": "dateTime_full_short",
                                        "l, M j": "date_full",
                                        "l, M j, Y": "date_full",
                                        "l, M j, Y g:ia": "dateTime_full_short",
                                        "M d": "MMMd",
                                        "M d, Y": "date_medium",
                                        "M d, Y g:ia": "dateTime_medium_short",
                                        "M d, Y ga": "dateTime_medium_short",
                                        "M j": "MMMd",
                                        "M j, Y": "date_medium",
                                        "M j, Y g:i A": "dateTime_medium_short",
                                        "M j, Y g:ia": "dateTime_medium_short",
                                        "M jS, g:ia": "dateTime_medium_short",
                                        "M y": "yMMM",
                                        "M Y": "yMMM",
                                        "M. d": "MMMd",
                                        "M. d, Y": "date_medium",
                                        "m/d": "Md",
                                        "m/d/Y g:ia": "dateTime_short_short",
                                        "m/d/y H:i:s": "dateTime_short_short",
                                        "n": "M",
                                        "n/j": "Md",
                                        "n/j, g:ia": "dateTime_short_short",
                                        "n/j/y": "date_short",
                                        "Y": "y"
                                    },
                                    "isLocaleInConfigerator": true,
                                    "CLDRConfigeratorFormats": {
                                        "dateFormats": {
                                            "full": "EEEE, d MMMM, y",
                                            "long": "d MMMM, y",
                                            "medium": "d MMM, y",
                                            "short": "d/M/yy"
                                        },
                                        "timeFormats": {
                                            "full": "HH:mm:ss zzzz",
                                            "long": "HH:mm:ss z",
                                            "medium": "HH:mm:ss",
                                            "short": "HH:mm"
                                        },
                                        "dateTimeFormats": {
                                            "full": "{0} {1}",
                                            "long": "{0} {1}",
                                            "medium": "{0} {1}",
                                            "short": "{0} {1}"
                                        },
                                        "availableFormats": {
                                            "Bh": "h 'giờ' B",
                                            "Bhm": "h:mm B",
                                            "Bhms": "h:mm:ss B",
                                            "E": "ccc",
                                            "EBhm": "h:mm B E",
                                            "EBhms": "h:mm:ss B E",
                                            "EHm": "HH:mm E",
                                            "EHms": "HH:mm:ss E",
                                            "Ed": "E, 'ngày' d",
                                            "Ehm": "h:mm a E",
                                            "Ehms": "h:mm:ss a E",
                                            "Gy": "y G",
                                            "GyMMM": "MMM y G",
                                            "GyMMMEd": "E, d MMM, y G",
                                            "GyMMMd": "d MMM, y G",
                                            "GyMd": "d/M/y G",
                                            "H": "HH 'giờ'",
                                            "Hm": "H:mm",
                                            "Hms": "HH:mm:ss",
                                            "Hmsv": "HH:mm:ss v",
                                            "Hmv": "HH:mm v",
                                            "M": "L",
                                            "MEd": "E, d/M",
                                            "MMM": "LLL",
                                            "MMMEd": "E, d MMM",
                                            "MMMMEd": "E, d MMMM",
                                            "MMMMW-count-other": "'tuần' W 'của' 'tháng' M",
                                            "MMMMd": "d MMMM",
                                            "MMMd": "d MMM",
                                            "MMdd": "dd-MM",
                                            "Md": "d/M",
                                            "d": "d",
                                            "h": "h a",
                                            "hm": "h:mm a",
                                            "hms": "h:mm:ss a",
                                            "hmsv": "h:mm:ss a v",
                                            "hmv": "h:mm a v",
                                            "mmss": "mm:ss",
                                            "ms": "mm:ss",
                                            "y": "y",
                                            "yM": "M/y",
                                            "yMEd": "E, d/M/y",
                                            "yMM": "'tháng' MM, y",
                                            "yMMM": "MMM y",
                                            "yMMMEd": "E, d MMM, y",
                                            "yMMMM": "MMMM 'năm' y",
                                            "yMMMd": "d MMM, y",
                                            "yMd": "d/M/y",
                                            "yQQQ": "QQQ y",
                                            "yQQQQ": "QQQQ 'năm' y",
                                            "yw-count-other": "'tuần' w 'của' 'năm' Y"
                                        }
                                    },
                                    "CLDRRegionalConfigeratorFormats": {
                                        "dateFormats": {
                                            "full": "EEEE, d MMMM, y",
                                            "long": "d MMMM, y",
                                            "medium": "d MMM, y",
                                            "short": "d/M/yy"
                                        },
                                        "timeFormats": {
                                            "full": "HH:mm:ss zzzz",
                                            "long": "HH:mm:ss z",
                                            "medium": "HH:mm:ss",
                                            "short": "HH:mm"
                                        },
                                        "dateTimeFormats": {
                                            "full": "{0} {1}",
                                            "long": "{0} {1}",
                                            "medium": "{0} {1}",
                                            "short": "{0} {1}"
                                        },
                                        "availableFormats": {
                                            "Bh": "h 'giờ' B",
                                            "Bhm": "h:mm B",
                                            "Bhms": "h:mm:ss B",
                                            "E": "ccc",
                                            "EBhm": "h:mm B E",
                                            "EBhms": "h:mm:ss B E",
                                            "EHm": "HH:mm E",
                                            "EHms": "HH:mm:ss E",
                                            "Ed": "E, 'ngày' d",
                                            "Ehm": "h:mm a E",
                                            "Ehms": "h:mm:ss a E",
                                            "Gy": "y G",
                                            "GyMMM": "MMM y G",
                                            "GyMMMEd": "E, d MMM, y G",
                                            "GyMMMd": "d MMM, y G",
                                            "GyMd": "d/M/y G",
                                            "H": "HH 'giờ'",
                                            "Hm": "H:mm",
                                            "Hms": "HH:mm:ss",
                                            "Hmsv": "HH:mm:ss v",
                                            "Hmv": "HH:mm v",
                                            "M": "L",
                                            "MEd": "E, d/M",
                                            "MMM": "LLL",
                                            "MMMEd": "E, d MMM",
                                            "MMMMEd": "E, d MMMM",
                                            "MMMMW-count-other": "'tuần' W 'của' 'tháng' M",
                                            "MMMMd": "d MMMM",
                                            "MMMd": "d MMM",
                                            "MMdd": "dd-MM",
                                            "Md": "d/M",
                                            "d": "d",
                                            "h": "h a",
                                            "hm": "h:mm a",
                                            "hms": "h:mm:ss a",
                                            "hmsv": "h:mm:ss a v",
                                            "hmv": "h:mm a v",
                                            "mmss": "mm:ss",
                                            "ms": "mm:ss",
                                            "y": "y",
                                            "yM": "M/y",
                                            "yMEd": "E, d/M/y",
                                            "yMM": "'tháng' MM, y",
                                            "yMMM": "MMM y",
                                            "yMMMEd": "E, d MMM, y",
                                            "yMMMM": "MMMM 'năm' y",
                                            "yMMMd": "d MMM, y",
                                            "yMd": "d/M/y",
                                            "yQQQ": "QQQ y",
                                            "yQQQQ": "QQQQ 'năm' y",
                                            "yw-count-other": "'tuần' w 'của' 'năm' Y"
                                        }
                                    },
                                    "CLDRToPHPSymbolConversion": {
                                        "G": "",
                                        "yyyy": "Y",
                                        "yy": "y",
                                        "y": "Y",
                                        "LLLLL": "M",
                                        "LLLL": "f",
                                        "LLL": "M",
                                        "LL": "m",
                                        "L": "n",
                                        "MMMMM": "M",
                                        "MMMM": "F",
                                        "MMM": "M",
                                        "MM": "m",
                                        "M": "n",
                                        "dd": "d",
                                        "d": "j",
                                        "ccccc": "D",
                                        "cccc": "l",
                                        "ccc": "D",
                                        "cc": "D",
                                        "c": "D",
                                        "EEEEE": "D",
                                        "EEEE": "l",
                                        "EEE": "D",
                                        "EE": "D",
                                        "E": "D",
                                        "aaaaa": "A",
                                        "aaaa": "A",
                                        "aaa": "A",
                                        "aa": "A",
                                        "a": "A",
                                        "bbbbb": "A",
                                        "bbbb": "A",
                                        "bbb": "A",
                                        "bb": "A",
                                        "b": "A",
                                        "BBBBB": "A",
                                        "BBBB": "A",
                                        "BBB": "A",
                                        "BB": "A",
                                        "B": "A",
                                        "HH": "H",
                                        "H": "G",
                                        "hh": "h",
                                        "h": "g",
                                        "K": "g",
                                        "mm": "i",
                                        "m": "i",
                                        "ss": "s",
                                        "s": "s",
                                        "z": "",
                                        "zz": "",
                                        "zzz": ""
                                    },
                                    "intlDateSpecialChars": {
                                        "cldrDelimiter": "'",
                                        "singleQuote": "'",
                                        "singleQuoteHolder": "*"
                                    }
                                },
                                3019
                            ],
                            [
                                "IsInternSite",
                                [],
                                {
                                    "is_intern_site": false
                                },
                                4517
                            ],
                            [
                                "EmojiConfig",
                                [],
                                {
                                    "pixelRatio": "1.5",
                                    "schemaAuth": "https://static.xx.fbcdn.net/images/emoji.php/v9",
                                    "hasEmojiPickerSearch": false
                                },
                                1421
                            ],
                            [
                                "CometMaxEnqueuedToastsSitevarConfig",
                                [],
                                {
                                    "max": 2
                                },
                                4763
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
                                "cr:2774",
                                [
                                    "LexicalUtils.prod"
                                ],
                                {
                                    "__rc": [
                                        "LexicalUtils.prod",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:5343",
                                [
                                    "useGroupsCometComposerMentionsDataSourceResolverConfig"
                                ],
                                {
                                    "__rc": [
                                        "useGroupsCometComposerMentionsDataSourceResolverConfig",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:1899533",
                                [
                                    "CometOnFBProfileVerificationBadge.react"
                                ],
                                {
                                    "__rc": [
                                        "CometOnFBProfileVerificationBadge.react",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:936168",
                                [
                                    "UFI2CometRelayBridge"
                                ],
                                {
                                    "__rc": [
                                        "UFI2CometRelayBridge",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:2139",
                                [
                                    "LexicalHashtag.prod"
                                ],
                                {
                                    "__rc": [
                                        "LexicalHashtag.prod",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:6943",
                                [
                                    "EventListenerImplForCacheStorage"
                                ],
                                {
                                    "__rc": [
                                        "EventListenerImplForCacheStorage",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:3024",
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
                                "cr:2046346",
                                [],
                                {
                                    "__rc": [
                                        null,
                                        "Aa3KmAPbxuCBH4WpFqo1GNdQE-c4zGYOormAq_zWd_KhBEa6SkxAQW8XciVmirXw9nrmTjHNaqN51rtJNuwmMrmM0dec9321wRWqtE3VmQZQ"
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:8905",
                                [
                                    "destroyOnUnloadWWW"
                                ],
                                {
                                    "__rc": [
                                        "destroyOnUnloadWWW",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:2682",
                                [
                                    "warningComet"
                                ],
                                {
                                    "__rc": [
                                        "warningComet",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:11202",
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
                                "cr:1105154",
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
                                "cr:1003267",
                                [
                                    "clearIntervalComet"
                                ],
                                {
                                    "__rc": [
                                        "clearIntervalComet",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:806696",
                                [
                                    "clearTimeoutComet"
                                ],
                                {
                                    "__rc": [
                                        "clearTimeoutComet",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:896461",
                                [
                                    "setIntervalComet"
                                ],
                                {
                                    "__rc": [
                                        "setIntervalComet",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:896462",
                                [
                                    "setIntervalComet"
                                ],
                                {
                                    "__rc": [
                                        "setIntervalComet",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:807042",
                                [
                                    "setTimeoutComet"
                                ],
                                {
                                    "__rc": [
                                        "setTimeoutComet",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:986633",
                                [
                                    "setTimeoutComet"
                                ],
                                {
                                    "__rc": [
                                        "setTimeoutComet",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:1183579",
                                [
                                    "InlineFbtResultImplComet"
                                ],
                                {
                                    "__rc": [
                                        "InlineFbtResultImplComet",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:3798",
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
                                "cr:1292365",
                                [
                                    "React-prod.classic"
                                ],
                                {
                                    "__rc": [
                                        "React-prod.classic",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:5277",
                                [
                                    "ReactDOM.classic.prod-or-profiling"
                                ],
                                {
                                    "__rc": [
                                        "ReactDOM.classic.prod-or-profiling",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:3976",
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
                                "cr:1094133",
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
                                "cr:1642797",
                                [
                                    "BanzaiComet"
                                ],
                                {
                                    "__rc": [
                                        "BanzaiComet",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:6895",
                                [
                                    "cometAsyncRequestHeaders"
                                ],
                                {
                                    "__rc": [
                                        "cometAsyncRequestHeaders",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:2548",
                                [
                                    "CometRelayEnvironmentWWW"
                                ],
                                {
                                    "__rc": [
                                        "CometRelayEnvironmentWWW",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:5888",
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
                                "cr:1024",
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
                                "cr:1829844",
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
                                "cr:1408565",
                                [
                                    "XCometContextualProfileControllerRouteBuilder"
                                ],
                                {
                                    "__rc": [
                                        "XCometContextualProfileControllerRouteBuilder",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "MarauderConfig",
                                [],
                                {
                                    "app_version": "1.0.0.0 (1012776817)",
                                    "gk_enabled": false
                                },
                                31
                            ],
                            [
                                "CurrentEnvironment",
                                [],
                                {
                                    "facebookdotcom": true,
                                    "messengerdotcom": false,
                                    "workplacedotcom": false,
                                    "instagramdotcom": false,
                                    "workdotmetadotcom": false,
                                    "horizondotmetadotcom": false
                                },
                                827
                            ],
                            [
                                "RTISubscriptionManagerConfig",
                                [],
                                {
                                    "config": {},
                                    "autobot": {},
                                    "assimilator": {},
                                    "unsubscribe_release": true,
                                    "bladerunner_www_sandbox": null,
                                    "is_intern": false
                                },
                                1081
                            ],
                            [
                                "RequestStreamE2EClientSamplingConfig",
                                [],
                                {
                                    "sampleRate": 100000,
                                    "methodToSamplingMultiplier": {
                                        "RTCSessionMessage": 10000,
                                        "Presence": 0.01,
                                        "FBGQLS:VOD_TICKER_SUBSCRIBE": 0.01,
                                        "FBGQLS:STORIES_TRAY_SUBSCRIBE": 100,
                                        "Collabri": 0.1,
                                        "FBGQLS:WORK_AVAILABILITY_STATUS_FANOUT_SUBSCRIBE": 0.1,
                                        "FBGQLS:GROUP_UNSEEN_ACTIVITY_SUBSCRIBE": 0.1,
                                        "FBGQLS:GROUP_RESET_UNSEEN_ACTIVITY_SUBSCRIBE": 0.1,
                                        "FBGQLS:INTERN_CALENDAR_UPDATE_SUBSCRIBE": 0.1,
                                        "SKY:gizmo_manage": 10000,
                                        "FBGQLS:FEEDBACK_LIKE_SUBSCRIBE": 10,
                                        "FBLQ:ios_huddle_listener": 1000,
                                        "FBGQLS:HUDDLE_USERS_REQUESTED_TO_SPEAK_COUNT_SUBSCRIBE": 1000
                                    }
                                },
                                4501
                            ],
                            [
                                "WebDriverConfig",
                                [],
                                {
                                    "isTestRunning": false,
                                    "isJestE2ETestRun": false,
                                    "isXRequestConfigEnabled": false,
                                    "auxiliaryServiceInfo": {},
                                    "testPath": null,
                                    "originHost": null
                                },
                                5332
                            ],
                            [
                                "DGWWebConfig",
                                [],
                                {
                                    "appId": "2220391788200892",
                                    "appVersion": "0",
                                    "dgwVersion": "2",
                                    "endpoint": "",
                                    "fbId": "61557504676830",
                                    "authType": ""
                                },
                                5508
                            ],
                            [
                                "NewsRegulationErrorMessageData",
                                [],
                                {
                                    "availableErrorCodes": [
                                        2216007,
                                        2216006
                                    ],
                                    "errorCodeToRegType": {
                                        "2216007": "c18",
                                        "2216006": "au00"
                                    },
                                    "learnMoreLinks": {
                                        "c18": {
                                            "regulated_user": "https://www.facebook.com/help/787040499275067",
                                            "user": "https://www.facebook.com/help/2579891418969617"
                                        },
                                        "au00": {
                                            "regulated_user": "https://www.facebook.com/help/787040499275067",
                                            "user": "https://www.facebook.com/help/2579891418969617"
                                        }
                                    },
                                    "appealLinks": {
                                        "c18": "https://www.facebook.com/help/contact/419859403337390"
                                    }
                                },
                                7133
                            ],
                            [
                                "DTSGInitialData",
                                [],
                                {
                                    "token": "NAcMJPT7Co2ZoEIK-02Cwxf6JgH0AuvdxnRGG3kPtMhq1Y38Kry0nWg:26:1712591601"
                                },
                                258
                            ],
                            [
                                "DTSGInitData",
                                [],
                                {
                                    "token": "NAcMJPT7Co2ZoEIK-02Cwxf6JgH0AuvdxnRGG3kPtMhq1Y38Kry0nWg:26:1712591601",
                                    "async_get_token": "AQybVMHc7WL4jhKoiG9mjiwNijQBut8ETxU0TnPtY6hsLch2:26:1712591601"
                                },
                                3515
                            ],
                            [
                                "FbtResultGK",
                                [],
                                {
                                    "shouldReturnFbtResult": true,
                                    "inlineMode": "NO_INLINE"
                                },
                                876
                            ],
                            [
                                "CometAltpayJsSdkIframeAllowedDomains",
                                [],
                                {
                                    "allowed_domains": [
                                        "https://live.adyen.com",
                                        "https://integration-facebook.payu.in",
                                        "https://facebook.payulatam.com",
                                        "https://secure.payu.com",
                                        "https://facebook.dlocal.com",
                                        "https://buy2.boku.com"
                                    ]
                                },
                                4920
                            ],
                            [
                                "WebLoomConfig",
                                [],
                                {
                                    "adaptive_config": {
                                        "interactions": {
                                            "modules": {
                                                "455": 1,
                                                "467": 1,
                                                "744": 1,
                                                "980": 1
                                            },
                                            "events": {
                                                "29818881.comet.error": 20.5,
                                                "29818881.comet.friending": 1.1,
                                                "29818881.comet.friending.suggestions": 2.1,
                                                "29818881.comet.fx.accounts_center.home": 2.8,
                                                "29818881.comet.gaming.games.canvas_player": 36.4,
                                                "29818881.comet.gaming.games.play": 2.7,
                                                "29818881.comet.group": 54.8,
                                                "29818881.comet.group.about": 1.8,
                                                "29818881.comet.group.permalink": 19.2,
                                                "29818881.comet.home": 652.9,
                                                "29818881.comet.marketplace.category": 1.1,
                                                "29818881.comet.marketplace.home": 3.4,
                                                "29818881.comet.marketplace.item": 9.6,
                                                "29818881.comet.mediaviewer.photo": 29.7,
                                                "29818881.comet.messenger.inbox": 49.9,
                                                "29818881.comet.post.single": 52,
                                                "29818881.comet.profile.collection.reels_tab": 4.7,
                                                "29818881.comet.profile.contextual_profile": 8.4,
                                                "29818881.comet.profile.logged_out": 5,
                                                "29818881.comet.profile.plus_logged_out": 39.2,
                                                "29818881.comet.profile.timeline.list": 226.1,
                                                "29818881.comet.reels.home": 28.1,
                                                "29818881.comet.search_results.default_tab": 5.3,
                                                "29818881.comet.settings.landing_page": 8.2,
                                                "29818881.comet.videos.tahoe": 1.2,
                                                "29818881.comet.wa.help.content": 26.1,
                                                "29818881.comet.watch.feed": 3.4,
                                                "29818881.comet.watch.injection": 17.4,
                                                "29818881.comet.watch.live.injection": 1.3,
                                                "29818881.public_chat_share_to_feed": 2.1,
                                                "29818882.comet.ActivityLog.CometActivityLogMainContentRoute": 3.7,
                                                "29818882.comet.birthday": 3,
                                                "29818882.comet.event.public.about": 2.8,
                                                "29818882.comet.friending": 9.7,
                                                "29818882.comet.friending.friendrequests": 6.9,
                                                "29818882.comet.friending.suggestions": 11.3,
                                                "29818882.comet.fx.accounts_center.home": 1.1,
                                                "29818882.comet.fx.accounts_center.section": 4.2,
                                                "29818882.comet.gaming.games": 3.4,
                                                "29818882.comet.gaming.games.canvas_player": 1.3,
                                                "29818882.comet.gaming.games.play": 7.3,
                                                "29818882.comet.group": 69.7,
                                                "29818882.comet.group.about": 1.2,
                                                "29818882.comet.group.media.photos": 2.6,
                                                "29818882.comet.group.members": 1.9,
                                                "29818882.comet.group.permalink": 15.8,
                                                "29818882.comet.groups.feed": 4.4,
                                                "29818882.comet.groups.pending_posts": 3.4,
                                                "29818882.comet.groups.viewer_content_pending": 1.1,
                                                "29818882.comet.home": 607.6,
                                                "29818882.comet.marketplace.category": 2.4,
                                                "29818882.comet.marketplace.composer": 1.4,
                                                "29818882.comet.marketplace.home": 28.2,
                                                "29818882.comet.marketplace.item": 30.8,
                                                "29818882.comet.marketplace.search": 24.8,
                                                "29818882.comet.marketplace.sellerProfileDialog": 2,
                                                "29818882.comet.marketplace.vehicles": 1.1,
                                                "29818882.comet.marketplace.you.selling": 2.5,
                                                "29818882.comet.mediaviewer.photo": 1180.7,
                                                "29818882.comet.mediaviewer.video": 10.5,
                                                "29818882.comet.memories": 4.8,
                                                "29818882.comet.messenger.inbox": 191.7,
                                                "29818882.comet.most_recent_feed": 1.4,
                                                "29818882.comet.post.single": 39.2,
                                                "29818882.comet.profile.collection.about": 8.6,
                                                "29818882.comet.profile.collection.about_contact_and_basic_info": 2.1,
                                                "29818882.comet.profile.collection.about_family_and_relationships": 1.1,
                                                "29818882.comet.profile.collection.about_work_and_education": 1.1,
                                                "29818882.comet.profile.collection.friends": 15.8,
                                                "29818882.comet.profile.collection.friends_recent": 1.3,
                                                "29818882.comet.profile.collection.photos": 52.2,
                                                "29818882.comet.profile.collection.photos_albums": 4.6,
                                                "29818882.comet.profile.collection.photos_by": 21.6,
                                                "29818882.comet.profile.collection.reels_tab": 5.1,
                                                "29818882.comet.profile.collection.videos": 1.1,
                                                "29818882.comet.profile.contextual_profile": 14,
                                                "29818882.comet.profile.media_set": 7.6,
                                                "29818882.comet.profile.plus_logged_out": 4.7,
                                                "29818882.comet.profile.timeline.list": 278.2,
                                                "29818882.comet.profile.timeline.videos": 1.5,
                                                "29818882.comet.reels.home": 55.8,
                                                "29818882.comet.save.saveDashboard": 2.1,
                                                "29818882.comet.search_results.default_tab": 66.3,
                                                "29818882.comet.search_results.entity_scoped": 7.3,
                                                "29818882.comet.sharedmediaviewer.media": 45.4,
                                                "29818882.comet.stories.create": 1.4,
                                                "29818882.comet.stories.viewer": 46.5,
                                                "29818882.comet.videos.tahoe": 10.5,
                                                "29818882.comet.wa.help.content": 1.9,
                                                "29818882.comet.watch.feed": 17.4,
                                                "29818882.comet.watch.injection": 15.6,
                                                "29818882.comet.watch.search": 1.4,
                                                "30605340.comet.group": 24,
                                                "30605354.comet.app": 981.8,
                                                "30605360.comet.profile.timeline.list": 11.7,
                                                "30605361.comet.composer.feed": 6.9,
                                                "30605361.comet.composer.profile": 12.8,
                                                "30605361.comet.composer.shareFeedToFeed": 20.5,
                                                "30605361.comet.composer.shareInstantGame": 1.1,
                                                "30605361.comet.composer.shareMemory": 1.1,
                                                "30605361.comet.dialog.BirthdayCometTodaysBirthdaysDialog.react": 7,
                                                "30605361.comet.dialog.CometCompatModalUniversal.react": 1.2,
                                                "30605361.comet.dialog.CometConfirmationDialogImpl.react": 29.2,
                                                "30605361.comet.dialog.CometEditFeedComposerDialog.react": 4.4,
                                                "30605361.comet.dialog.CometFocusedStoryDialogViewRoot.react": 217.4,
                                                "30605361.comet.dialog.CometGroupResharesDialog.react": 7.3,
                                                "30605361.comet.dialog.CometMediaViewerDeleteConfirmationDialog.react": 2.6,
                                                "30605361.comet.dialog.CometMessengerResharesDialog.react": 4.4,
                                                "30605361.comet.dialog.CometOnBeforeUnloadDialog.react": 4.8,
                                                "30605361.comet.dialog.CometPrivacySelectorDialog.react": 2.8,
                                                "30605361.comet.dialog.CometResharesDialog.react": 1.9,
                                                "30605361.comet.dialog.CometSaveSelectCollectionDialog.react": 3,
                                                "30605361.comet.dialog.CometUFIReactionsDialog.react": 27,
                                                "30605361.comet.dialog.CometUnifiedShareSheetDialog.react": 6.5,
                                                "30605361.comet.dialog.GroupCometComposerCreateDialog.react": 25.8,
                                                "30605361.comet.dialog.MWChatForwardDialog.react": 6.6,
                                                "30605361.comet.dialog.MWEBRestoreDialogWrapper.react": 4.6,
                                                "30605361.comet.emojipicker": 5.9,
                                                "30605361.comet.feed.story.menu": 45.2,
                                                "30605361.comet.jewel.megamenu": 3.8,
                                                "30605361.comet.jewel.messenger": 528.7,
                                                "30605361.comet.jewel.notification": 269.7,
                                                "30605361.comet.jewel.settings": 97.5,
                                                "30605361.comet.popover.CometActivityLogActionMenu.react": 2.6,
                                                "30605361.comet.popover.CometHomeChatSettings.react": 5.7,
                                                "30605361.comet.popover.CometMarketplaceYouFeedCardMoreMenu.react": 1.7,
                                                "30605361.comet.popover.CometNotificationsActionsMenu.react": 3.2,
                                                "30605361.comet.popover.CometNotificationsDropdownMenuContainer.react": 6.8,
                                                "30605361.comet.popover.CometTabMenu.react": 4.5,
                                                "30605361.comet.popover.CometUFICommentMenu.react": 8.3,
                                                "30605361.comet.popover.CometUFICommentRenderingIntentSelectorMenu.react": 19.8,
                                                "30605361.comet.popover.CometUFIEmojiPickerPopoverForLexical.react": 6.6,
                                                "30605361.comet.popover.CometUFIShareActionLinkMenu.react": 39.4,
                                                "30605361.comet.popover.CometVerificationBadgeInfoPopover.react": 7.9,
                                                "30605361.comet.popover.CometVideoHomeVideoContextMenuContents.react": 1.5,
                                                "30605361.comet.popover.FBReelsMenu.react": 3.7,
                                                "30605361.comet.popover.GroupsCometFeedSortingSwitcherMenu.react": 1.2,
                                                "30605361.comet.popover.GroupsCometMoreActionMenu.react": 1.7,
                                                "30605361.comet.popover.MWChatReactionsMenu.react": 87.7,
                                                "30605361.comet.popover.MWChatStickersFlyout.react": 1.5,
                                                "30605361.comet.popover.MWThreadListHoverButtonDropdownMenu.react": 14.8,
                                                "30605361.comet.popover.MWV2ComposerEmojiPickerForJSResource": 19.1,
                                                "30605361.comet.popover.MWV2ComposerOverflowMenu.react": 2,
                                                "30605361.comet.popover.MWV2ContextualActionsMenu.react": 26.1,
                                                "30605361.comet.popover.MWV2HeaderSettingsMenu.react": 19.7,
                                                "30605361.comet.popover.ProfileCometActiveFriendMenu.react": 6.7,
                                                "30605361.comet.popover.ProfileCometAppCollectionMediaActionsMenu.react": 2.2,
                                                "30605361.comet.popover.ProfileCometHeaderActionBarMoreMenu.react": 8.6,
                                                "30605361.comet.popover.ProfileCometProfilePictureEditMenu.react": 3.1,
                                                "30605361.comet.popover.ProfileCometProfilePictureViewMenu.react": 5.4,
                                                "30605361.comet.popover.marketplace.pdpSaveButton": 1.2,
                                                "30605361.comet.search_scoped.group": 3.1,
                                                "30605361.mwp.dialog.MWChatBlockWarningCardDialog.react": 1.1,
                                                "30605361.mwp.dialog.MWChatDeleteConversationDialog.react": 8.1,
                                                "30605361.mwp.dialog.MWV2MediaViewer.react": 27.9,
                                                "30605361.mwp.dialog.MWV2RemoveMessageDialog.react": 12,
                                                "30605361.mwp.dialog.MWXConfirmationDialog.react": 5.2,
                                                "30605363.comet.gaming.games.canvas_player": 1.2,
                                                "30605374.comet.home": 4.2,
                                                "30605374.comet.mediaviewer.photo": 3.3,
                                                "30605374.comet.post.single": 2.4,
                                                "30605374.comet.profile.timeline.list": 10.2,
                                                "30605380.comet.app": 706.9,
                                                "30605380.comet.friending": 1.2,
                                                "30605380.comet.group.members": 1.1,
                                                "30605380.comet.home": 31.1,
                                                "30605380.comet.marketplace.item": 1.9,
                                                "30605380.comet.profile.collection.friends": 3.3,
                                                "30605380.comet.profile.timeline.list": 19.1,
                                                "30605384.comet.app": 899.9,
                                                "30605384.comet.messenger.inbox": 141.1,
                                                "30605391.comet.profile.timeline.videos": 6.4,
                                                "30607516.comet.jewel.message_requests": 7.4,
                                                "30608422.comet.app": 2.6,
                                                "30609204.comet.group": 1.3,
                                                "30609204.comet.home": 30.6,
                                                "30609204.comet.post.single": 2,
                                                "30609204.comet.profile.timeline.list": 10.6,
                                                "30609204.comet.reels.home": 1.5,
                                                "30612548.comet.reels.reel": 1376.7,
                                                "30615205.comet.error": 7.9,
                                                "30615205.comet.friending": 1.5,
                                                "30615205.comet.friending.suggestions": 1.8,
                                                "30615205.comet.gaming.games.play": 2.1,
                                                "30615205.comet.group": 34.6,
                                                "30615205.comet.group.about": 1.2,
                                                "30615205.comet.group.permalink": 11.7,
                                                "30615205.comet.home": 437.1,
                                                "30615205.comet.marketplace.home": 2.2,
                                                "30615205.comet.marketplace.item": 6.1,
                                                "30615205.comet.mediaviewer.photo": 15.6,
                                                "30615205.comet.post.single": 28.2,
                                                "30615205.comet.profile.collection.reels_tab": 3.3,
                                                "30615205.comet.profile.contextual_profile": 5.8,
                                                "30615205.comet.profile.timeline.list": 148.9,
                                                "30615205.comet.reels.home": 10.8,
                                                "30615205.comet.search_results.default_tab": 3.8,
                                                "30615205.comet.settings.landing_page": 5.6,
                                                "30615205.comet.videos.tahoe": 1.2,
                                                "30615205.comet.watch.feed": 2.5,
                                                "30615205.comet.watch.injection": 6.6,
                                                "30615205.comet.watch.live.injection": 1.3,
                                                "30615205.public_chat_share_to_feed": 1.6,
                                                "30615365.comet.profile.timeline.list": 9.6,
                                                "30615438.comet.group": 1.5,
                                                "30615438.comet.home": 2,
                                                "64231865.zenon.groupcall": 12.7
                                            }
                                        },
                                        "qpl": {
                                            "modules": {},
                                            "events": {}
                                        },
                                        "modules": null,
                                        "events": null
                                    }
                                },
                                4171
                            ],
                            [
                                "DataStoreConfig",
                                [],
                                {
                                    "expandoKey": "__FB_STORE",
                                    "useExpando": true
                                },
                                2915
                            ],
                            [
                                "cr:2680",
                                [
                                    "WebPixelRatio"
                                ],
                                {
                                    "__rc": [
                                        "WebPixelRatio",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:7387",
                                [
                                    "requestIdleCallbackWWW"
                                ],
                                {
                                    "__rc": [
                                        "requestIdleCallbackWWW",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:2180",
                                [
                                    "LexicalSelection.prod"
                                ],
                                {
                                    "__rc": [
                                        "LexicalSelection.prod",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:983844",
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
                                "cr:1072546",
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
                                "cr:1072547",
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
                                "cr:1072549",
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
                                "cr:5278",
                                [
                                    "ReactDOM-profiling.classic"
                                ],
                                {
                                    "__rc": [
                                        "ReactDOM-profiling.classic",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:6016",
                                [
                                    "NavigationMetricsWWW"
                                ],
                                {
                                    "__rc": [
                                        "NavigationMetricsWWW",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:7384",
                                [
                                    "cancelIdleCallbackWWW"
                                ],
                                {
                                    "__rc": [
                                        "cancelIdleCallbackWWW",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:1268629",
                                [
                                    "setTimeoutCometLoggingPri"
                                ],
                                {
                                    "__rc": [
                                        "setTimeoutCometLoggingPri",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:1268630",
                                [
                                    "setTimeoutCometSpeculative"
                                ],
                                {
                                    "__rc": [
                                        "setTimeoutCometSpeculative",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "FunnelLoggerConfig",
                                [],
                                {
                                    "freq": {
                                        "WWW_MESSENGER_VIDEO_CHAT_LINKS_FUNNEL": 1,
                                        "PIE_MANAGER_HIRING_HUB_FUNNEL": 1,
                                        "WWW_ESCALATION_TOOLS_NOTIFICATIONS_PAGE_FUNNEL": 1,
                                        "WWW_ONCALL_VIEW_FUNNEL": 1,
                                        "WWW_MESSENGER_GROUP_ESCALATION_FUNNEL": 10,
                                        "WWW_SPATIAL_REACTION_PRODUCTION_FUNNEL": 1,
                                        "CREATIVE_STUDIO_CREATION_FUNNEL": 1,
                                        "WWW_CANVAS_AD_CREATION_FUNNEL": 1,
                                        "WWW_CANVAS_EDITOR_FUNNEL": 1,
                                        "WWW_LINK_PICKER_DIALOG_FUNNEL": 1,
                                        "WWW_MEME_PICKER_DIALOG_FUNNEL": 1,
                                        "WWW_LEAD_GEN_FORM_CREATION_FUNNEL": 1,
                                        "WWW_LEAD_GEN_FORM_EDITOR_FUNNEL": 1,
                                        "WWW_LEAD_GEN_DESKTOP_AD_UNIT_FUNNEL": 1,
                                        "WWW_LEAD_GEN_MSITE_AD_UNIT_FUNNEL": 1,
                                        "WWW_CAMPFIRE_COMPOSER_UPSELL_FUNNEL": 1,
                                        "WWW_PMT_FUNNEL": 1,
                                        "WWW_PULSE_FUNNEL": 1,
                                        "WWW_ORGTOOL_FUNNEL": 1,
                                        "WWW_RECRUITING_PRODUCTS_ATTRIBUTION_FUNNEL": 1,
                                        "WWW_RECRUITING_PRODUCTS_FUNNEL": 1,
                                        "WWW_RECRUITING_SEARCH_FUNNEL": 1,
                                        "WWW_RECRUITING_BULK_EMAIL_FUNNEL": 1,
                                        "WWW_RECRUITING_LEAVE_HANDLER_FUNNEL": 1,
                                        "WWW_EXAMPLE_FUNNEL": 1,
                                        "WWW_REACTIONS_BLINGBAR_NUX_FUNNEL": 1,
                                        "WWW_REACTIONS_NUX_FUNNEL": 1,
                                        "WWW_COMMENT_REACTIONS_NUX_FUNNEL": 1,
                                        "WWW_MESSENGER_SHARE_TO_FB_FUNNEL": 10,
                                        "POLYGLOT_MAIN_FUNNEL": 1,
                                        "MSITE_EXAMPLE_FUNNEL": 10,
                                        "WWW_FEED_SHARE_DIALOG_FUNNEL": 100,
                                        "MSITE_AD_BREAKS_ONBOARDING_FLOW_FUNNEL": 1,
                                        "MSITE_FEED_ALBUM_CTA_FUNNEL": 10,
                                        "MSITE_FEED_SHARE_DIALOG_FUNNEL": 100,
                                        "MSITE_COMMENT_TYPING_FUNNEL": 500,
                                        "MSITE_HASHTAG_PROMPT_FUNNEL": 1,
                                        "WWW_SEARCH_AWARENESS_LEARNING_NUX_FUNNEL": 1,
                                        "WWW_CONSTITUENT_TITLE_UPSELL_FUNNEL": 1,
                                        "MTOUCH_FEED_MISSED_STORIES_FUNNEL": 10,
                                        "WWW_UFI_SHARE_LINK_FUNNEL": 1,
                                        "WWW_CMS_SEARCH_FUNNEL": 1,
                                        "GAMES_QUICKSILVER_FUNNEL": 1,
                                        "SOCIAL_SEARCH_CONVERSION_WWW_FUNNEL": 1,
                                        "SOCIAL_SEARCH_DASHBOARD_WWW_FUNNEL": 1,
                                        "SRT_USER_FLOW_FUNNEL": 1,
                                        "MSITE_PPD_FUNNEL": 1,
                                        "WWW_PAGE_CREATION_FUNNEL": 1,
                                        "NT_EXAMPLE_FUNNEL": 1,
                                        "WWW_LIVE_VIEWER_TIPJAR_FUNNEL": 1,
                                        "FACECAST_BROADCASTER_FUNNEL": 1,
                                        "WWW_FUNDRAISER_CREATION_FUNNEL": 1,
                                        "WWW_FUNDRAISER_EDIT_FUNNEL": 1,
                                        "WWW_OFFERS_SIMPLE_COMPOSE_FUNNEL": 1,
                                        "QP_TOOL_FUNNEL": 1,
                                        "WWW_OFFERS_SIMPLE_COMPOSE_POST_LIKE_FUNNEL": 1,
                                        "COLLEGE_COMMUNITY_NUX_ONBOARDING_FUNNEL": 1,
                                        "CASUAL_GROUP_PICKER_FUNNEL": 1,
                                        "TOPICS_TO_FOLLOW_FUNNEL": 1,
                                        "WWW_MESSENGER_SEARCH_SESSION_FUNNEL": 1,
                                        "WWW_LIVE_PRODUCER_FUNNEL": 1,
                                        "FX_PLATFORM_INVITE_JOIN_FUNNEL": 1,
                                        "CREATIVE_STUDIO_HUB_FUNNEL": 1,
                                        "WWW_SEE_OFFERS_CTA_NUX_FUNNEL": 1,
                                        "WWW_ADS_TARGETING_AUDIENCE_MANAGER_FUNNEL": 1,
                                        "WWW_AD_BREAKS_ONBOARDING_FUNNEL": 1,
                                        "WWW_AD_BREAK_HOME_ONBOARDING_FUNNEL": 1,
                                        "WWW_NOTIFS_UP_NEXT_FUNNEL": 10,
                                        "ADS_VIDEO_CAPTION_FUNNEL": 1,
                                        "KEYFRAMES_FUNNEL": 500,
                                        "SEARCH_ADS_WWW_FUNNEL": 1,
                                        "WWW_ALT_TEXT_COMPOSER_FUNNEL": 1,
                                        "BUSINESS_PAYMENTS_MERCHANT_ONBOARDING_FUNNEL": 1,
                                        "MERCHANT_PAYMENTS_MERCHANT_ONBOARDING_FUNNEL": 1,
                                        "SELLER_EXPERIENCE_ONBOARDING_NEW_FUNNEL": 1,
                                        "SELLER_EXPERIENCE_PAYOUT_SETUP_NEW_FUNNEL": 1,
                                        "SELLER_EXPERIENCE_SHOP_MANAGEMENT_FUNNEL": 1,
                                        "WWW_BUSINESS_CREATION_FUNNEL": 1,
                                        "WWW_BUSINESS_VERIFICATION_FUNNEL": 1,
                                        "WWW_APP_REVIEW_BUSINESS_VERIFICATION_FUNNEL": 1,
                                        "SELLER_EXPERIENCE_MIGRATION_FUNNEL": 1,
                                        "SELLER_EXPERIENCE_PAYOUT_SETUP_FUNNEL": 1,
                                        "PAYOUT_ONBOARDING_FUNNEL": 1,
                                        "SERVICES_INSTANT_BOOKING_SETTINGS_FUNNEL": 1,
                                        "SERVICES_FB_APPOINTMENTS_CTA_FULL_SETUP_FUNNEL": 1,
                                        "SERVICES_FB_APPOINTMENTS_CTA_CREATION_FUNNEL": 1,
                                        "FB_NEO_ONBOARDING_FUNNEL": 1,
                                        "FB_NEO_FRIENDING_FUNNEL": 1,
                                        "WWW_MESSENGER_CONTENT_SEARCH_FUNNEL": 1,
                                        "SEARCH_FUNNEL": 1,
                                        "SHADOW_SEARCH_FUNNEL": 1,
                                        "SHADOW_EARLY_END_SEARCH_FUNNEL": 1,
                                        "UNIDASH_EDIT_WIDGET_FUNNEL": 1,
                                        "PRIVATE_COMMENT_COMPOSER_FUNNEL": 1,
                                        "WEB_RTC_SCREEN_SHARING_FUNNEL": 1,
                                        "CHECKOUT_EXPERIENCES_FUNNEL": 1,
                                        "CHECKOUT_EXPERIENCES_SELLER_FUNNEL": 1,
                                        "WWW_SERVICES_INSTANT_BOOKING_CONSUMER_FUNNEL": 1,
                                        "WWW_SERVICES_BOOK_APPOINTMENT_CONSUMER_FUNNEL": 10,
                                        "WWW_SPHERICAL_DIRECTOR_FUNNEL": 1,
                                        "NATIVE_SUPPORT_FUNNEL": 1,
                                        "WWW_PRESENCE_FUNNEL": 1,
                                        "MESSENGER_UNIVERSAL_SEARCH_FUNNEL": 1,
                                        "MESSENGER_SECONDARY_SEARCH_FUNNEL": 1,
                                        "WORK_CHAT_SEARCH_FUNNEL": 1,
                                        "PRIVACY_SHORTCUTS_FUNNEL": 1,
                                        "PRIVACY_ACCESS_HUB_FUNNEL": 1,
                                        "WWW_POLITICIAN_OFFICE_SETTING_FUNNEL": 1,
                                        "WWW_CIVIC_ACTION_POST_INVITE_FUNNEL": 1,
                                        "WWW_MESSENGER_SHARE_FILE_PREVIEW_FUNNEL": 1,
                                        "ALL_VOICES_FUNNEL": 1,
                                        "AEC_APPLICATION_FUNNEL": 1,
                                        "INSTANT_EXPERIENCES_MINDBODY_FUNNEL": 1,
                                        "WWW_LAUNCHPAD_ONBOARDING_FUNNEL": 1,
                                        "GIZMO_VCPANEL_CALL_START_FUNNEL": 1,
                                        "WWW_FB_CHAT_NEW_SETTINGS_MENU_FUNNEL": 1,
                                        "KAIOS_REG_CONTACT_IMPORTER_FUNNEL": 1,
                                        "MAP_WEB_FUNNEL": 1,
                                        "SOCIAL_VR_INTERACTIVE_THREE_SIXTY_FUNNEL": 1,
                                        "WWW_SNOWLIFT_ACTIONS_FUNNEL": 1,
                                        "SVC_DEPLOYMENT_ONBOARDING_FUNNEL": 1,
                                        "FHT_FUNNEL": 1,
                                        "default": 1000
                                    }
                                },
                                1271
                            ],
                            [
                                "BanzaiConfig",
                                [],
                                {
                                    "MAX_SIZE": 10000,
                                    "MAX_WAIT": 150000,
                                    "MIN_WAIT": null,
                                    "RESTORE_WAIT": 150000,
                                    "blacklist": [
                                        "time_spent"
                                    ],
                                    "disabled": false,
                                    "gks": {
                                        "boosted_pagelikes": true,
                                        "mercury_send_error_logging": true,
                                        "platform_oauth_client_events": true,
                                        "sticker_search_ranking": true
                                    },
                                    "known_routes": [
                                        "artillery_javascript_actions",
                                        "artillery_javascript_trace",
                                        "artillery_logger_data",
                                        "logger",
                                        "falco",
                                        "gk2_exposure",
                                        "js_error_logging",
                                        "loom_trace",
                                        "marauder",
                                        "perfx_custom_logger_endpoint",
                                        "qex",
                                        "require_cond_exposure_logging",
                                        "metaconfig_exposure"
                                    ],
                                    "should_drop_unknown_routes": true,
                                    "should_log_unknown_routes": false
                                },
                                7
                            ],
                            [
                                "cr:694370",
                                [
                                    "requestIdleCallbackComet"
                                ],
                                {
                                    "__rc": [
                                        "requestIdleCallbackComet",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:5695",
                                [
                                    "EventListenerWWW"
                                ],
                                {
                                    "__rc": [
                                        "EventListenerWWW",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:8909",
                                [
                                    "ReactFiberErrorDialogWWW"
                                ],
                                {
                                    "__rc": [
                                        "ReactFiberErrorDialogWWW",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:692209",
                                [
                                    "cancelIdleCallbackComet"
                                ],
                                {
                                    "__rc": [
                                        "cancelIdleCallbackComet",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:1353359",
                                [
                                    "CometEventListener"
                                ],
                                {
                                    "__rc": [
                                        "CometEventListener",
                                        null
                                    ]
                                },
                                -1
                            ],
                            [
                                "IntlNumberTypeProps",
                                [
                                    "IntlCLDRNumberType01"
                                ],
                                {
                                    "module": {
                                        "__m": "IntlCLDRNumberType01"
                                    }
                                },
                                7027
                            ],
                            [
                                "CurrentUserInitialData",
                                [],
                                {
                                    "ACCOUNT_ID": "61557504676830",
                                    "USER_ID": "61557504676830",
                                    "NAME": "Lý Mai",
                                    "SHORT_NAME": "Lý",
                                    "IS_BUSINESS_PERSON_ACCOUNT": false,
                                    "HAS_SECONDARY_BUSINESS_PERSON": false,
                                    "IS_FACEBOOK_WORK_ACCOUNT": false,
                                    "IS_MESSENGER_ONLY_USER": false,
                                    "IS_DEACTIVATED_ALLOWED_ON_MESSENGER": false,
                                    "IS_MESSENGER_CALL_GUEST_USER": false,
                                    "IS_WORK_MESSENGER_CALL_GUEST_USER": false,
                                    "IS_WORKROOMS_USER": false,
                                    "APP_ID": "2220391788200892",
                                    "IS_BUSINESS_DOMAIN": false
                                },
                                270
                            ],
                            [
                                "QuickMarkersConfig",
                                [],
                                {
                                    "pageLoadEventId": "7358014106295232747",
                                    "pageLoadScriptPath": "XGraphQLAPIController:CommentListComponentsRootQuery",
                                    "sampleWeight": null
                                },
                                4953
                            ],
                            [
                                "DynamicUFIReactionTypes",
                                [],
                                {
                                    "reactions": {
                                        "1635855486666999": {
                                            "color": "#0866FF",
                                            "display_name": "Thích",
                                            "is_deprecated": false,
                                            "is_visible": true,
                                            "name": "like",
                                            "type": 1
                                        },
                                        "1678524932434102": {
                                            "color": "#f33e58",
                                            "display_name": "Yêu thích",
                                            "is_deprecated": false,
                                            "is_visible": true,
                                            "name": "love",
                                            "type": 2
                                        },
                                        "869508936487422": {
                                            "color": "#f0ba15",
                                            "display_name": "Ảnh selfie",
                                            "is_deprecated": true,
                                            "is_visible": false,
                                            "name": "selfie",
                                            "type": 13
                                        },
                                        "1663186627268800": {
                                            "color": "#7e64c4",
                                            "display_name": "Biết ơn",
                                            "is_deprecated": false,
                                            "is_visible": true,
                                            "name": "dorothy",
                                            "type": 11
                                        },
                                        "899779720071651": {
                                            "color": "#ec7ebd",
                                            "display_name": "Tự hào",
                                            "is_deprecated": false,
                                            "is_visible": true,
                                            "name": "toto",
                                            "type": 12
                                        },
                                        "115940658764963": {
                                            "color": "#f7b125",
                                            "display_name": "Haha",
                                            "is_deprecated": false,
                                            "is_visible": true,
                                            "name": "haha",
                                            "type": 4
                                        },
                                        "1667835766830853": {
                                            "color": "#f0ba15",
                                            "display_name": "Chúc mừng",
                                            "is_deprecated": true,
                                            "is_visible": false,
                                            "name": "yay",
                                            "type": 5
                                        },
                                        "478547315650144": {
                                            "color": "#f7b125",
                                            "display_name": "Wow",
                                            "is_deprecated": false,
                                            "is_visible": true,
                                            "name": "wow",
                                            "type": 3
                                        },
                                        "1536130110011063": {
                                            "color": "#f0ba15",
                                            "display_name": "Khó hiểu",
                                            "is_deprecated": true,
                                            "is_visible": false,
                                            "name": "confused",
                                            "type": 10
                                        },
                                        "613557422527858": {
                                            "color": "#f7b125",
                                            "display_name": "Thương thương",
                                            "is_deprecated": false,
                                            "is_visible": true,
                                            "name": "support",
                                            "type": 16
                                        },
                                        "908563459236466": {
                                            "color": "#f7b125",
                                            "display_name": "Buồn",
                                            "is_deprecated": false,
                                            "is_visible": true,
                                            "name": "sorry",
                                            "type": 7
                                        },
                                        "444813342392137": {
                                            "color": "#e9710f",
                                            "display_name": "Phẫn nộ",
                                            "is_deprecated": false,
                                            "is_visible": true,
                                            "name": "anger",
                                            "type": 8
                                        },
                                        "938644726258608": {
                                            "color": "#f0ba15",
                                            "display_name": "Bày tỏ cảm xúc",
                                            "is_deprecated": true,
                                            "is_visible": false,
                                            "name": "flame",
                                            "type": 14
                                        },
                                        "1609920819308489": {
                                            "color": "#f0ba15",
                                            "display_name": "Bày tỏ cảm xúc",
                                            "is_deprecated": true,
                                            "is_visible": false,
                                            "name": "plane",
                                            "type": 15
                                        }
                                    },
                                    "ordering": [
                                        "1635855486666999",
                                        "1678524932434102",
                                        "613557422527858",
                                        "115940658764963",
                                        "478547315650144",
                                        "908563459236466",
                                        "444813342392137"
                                    ]
                                },
                                6492
                            ],
                            [
                                "DynamicUFIReactionsKeyframesAssets",
                                [],
                                {
                                    "likeAction": "https://static.xx.fbcdn.net/rsrc.php/yg/r/DUjm2v1u572.kf",
                                    "reactions": {
                                        "1635855486666999": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An_NYk94x95Kypus5FJQ4k1oKEtko7-rUveEhwXytks318UoxoopBczHucoGDTjX4YcuAmIDkUw9SWBKhz7XYoAsQO_zxmWdkseO4YNdrvYmnIdmeAk.kf?ccb=10-5&oh=00_AfC4N59wnCTXy-mqcto-H4aFf0t_dEdWoIbTiBnBpDEN0A&oe=66447038&_nc_sid=7da55a",
                                        "1678524932434102": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9Tph7xL5aYi3BTTpVl2ow-l1vEv0-qYrBxereq6t6fWgcNnxeyJLsd3DuGnbCLdLFmcvvxn5ivo85wlrIv-EZhT1EucYZ-qoMW0ahYWHGpBBoqSjw.kf?ccb=10-5&oh=00_AfDQ-6lecXmTlchQ-RyfLcosRP1EUCa4krksCPKuOdWCvw&oe=66444D81&_nc_sid=7da55a",
                                        "1663186627268800": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An8KSKhioMIUVSZ4NYh8JnAchGmGQVDA71Hulkn5JQZsO-ejSYcV2dWPMQo-ZhSa71MfFqgrDHlCASWFxgbtV3pYQqVdSus0zicQO6_n.kf?ccb=10-5&oh=00_AfCryD4w6qlNxvWD1FILq7LPgmhC1T5y2G7gD2h4aBE2Cw&oe=66446CA6&_nc_sid=7da55a",
                                        "899779720071651": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An8UpDtYTxwRfyFUAQkYpPLVzCcFZAyT58b4mM9QRn-9IZWdHfcWsX1lOuHAsupZu8HCFEX8uobe6VdR6H9B8v2Z_FzSMfB8MYN36w.kf?ccb=10-5&oh=00_AfAsVG9hbKKvVXSRWak48KXzL-5CW3MswGBHE7dntg0lMg&oe=66444F30&_nc_sid=7da55a",
                                        "115940658764963": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9yyyXsW_c8BzV1_m0x9WqIPc7IKsshuStlldoUJeshdwMKRkmQmdPEGGwMopV9sH85YDKihkJ8DjNhx1wb2IaUuEOGzE_ji5F9MEXs_50bbA-IXQ.kf?ccb=10-5&oh=00_AfDHdIX2WR5sWRP3EbJwkmXXizlWvkkxyozcLRGko3OFmw&oe=664454A5&_nc_sid=7da55a",
                                        "478547315650144": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9Ob_EAguyCtqplSNOuikWQ6JjlxIh8vYoEgMXvR0CwneLvNdYwV-1NZgwJfR4aZ4QXhIpQUZxunwGdGubGw20jp-9DikfLbRVh-i4tobncZg9LGpE.kf?ccb=10-5&oh=00_AfBH4f_8b9YpKyqgriHL1hsfvrjLf57CHW4C13NN_Uqp1g&oe=66444171&_nc_sid=7da55a",
                                        "613557422527858": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An-iEpi04A6D-3XVq3wsUCtKdkB4w6IdurXeouCv4FsHYljtXw-fLrmbfC8B8zH5fPrckxLdEzR7V7dfidlNcrNoGsJWxiPDnzyNK-npl_KrJieMlg.kf?ccb=10-5&oh=00_AfAfoDjoOK-htcJ9ZDVYLBbUr_TNAdP_o_8P-R59OVhhig&oe=664475AE&_nc_sid=7da55a",
                                        "908563459236466": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An9UFu6eXdDopP-SnPAhX-9SngOH_VeoYgHIGK6re6qbARX_PMcNl8Z14QPPFnVzbcfOQwxJxX5q-H5Fy3602EbOrVHhr1m4VSMXypn3fj2NSJongRg.kf?ccb=10-5&oh=00_AfDcHEN-Lj4ZCyxGPwBZoihFPCZSsZd9ZUgr77Gp74G5ag&oe=664467C8&_nc_sid=7da55a",
                                        "444813342392137": "https://scontent.fsgn2-11.fna.fbcdn.net/m1/v/t6/An919EwtdC17ceBi2men2TIR0UhNUwitUvpE61_Jbs44ggFt3mvLWkKiHP_CSmw72ohKdyEscSIBof6y1FeS57I3kGfh5tg96jndT5mnnEuJlpXuvuUj.kf?ccb=10-5&oh=00_AfD72uYo4bK4mUP0nsihQdCNdL-Eo6WbQt4XeEsX2z2zjw&oe=664465A4&_nc_sid=7da55a"
                                    },
                                    "initialProgress": {
                                        "115940658764963": 0.37,
                                        "908563459236466": 0.75
                                    }
                                },
                                6513
                            ],
                            [
                                "DateFormatConfig",
                                [],
                                {
                                    "numericDateOrder": [
                                        "d",
                                        "m",
                                        "y"
                                    ],
                                    "numericDateSeparator": "/",
                                    "shortDayNames": [
                                        "T2",
                                        "T3",
                                        "T4",
                                        "T5",
                                        "T6",
                                        "T7",
                                        "CN"
                                    ],
                                    "narrowDayNames": [
                                        "T2",
                                        "T3",
                                        "Thứ Tư",
                                        "T5",
                                        "T6",
                                        "Thứ Bảy",
                                        "CN"
                                    ],
                                    "timeSeparator": ":",
                                    "weekStart": 6,
                                    "formats": {
                                        "D": "D",
                                        "D g:ia": "D G:i",
                                        "D M d": "j F",
                                        "D M d, Y": "j F Y",
                                        "D M j": "j F",
                                        "D M j, g:ia": "j F G:i",
                                        "D M j, y": "j F Y",
                                        "D M j, Y g:ia": "j F Y G:i",
                                        "D, M j, Y": "j F Y",
                                        "F d": "j F",
                                        "F d, Y": "j F Y",
                                        "F g": "j F",
                                        "F j": "j F",
                                        "F j, Y": "j F Y",
                                        "F j, Y @ g:i A": "j F Y G:i",
                                        "F j, Y g:i a": "j F Y G:i",
                                        "F jS": "j F",
                                        "F jS, g:ia": "j F G:i",
                                        "F jS, Y": "j F Y",
                                        "F Y": "F Y",
                                        "g A": "G",
                                        "g:i": "G:i",
                                        "g:i A": "G:i",
                                        "g:i a": "G:i",
                                        "g:iA": "G:i",
                                        "g:ia": "G:i",
                                        "g:ia F jS, Y": "j F Y G:i",
                                        "g:iA l, F jS": "j F Y G:i",
                                        "g:ia M j": "j F G:i",
                                        "g:ia M jS": "j F G:i",
                                        "g:ia, F jS": "j F G:i",
                                        "g:iA, l M jS": "j F Y G:i",
                                        "g:sa": "G:i",
                                        "H:I - M d, Y": "j F Y G:i",
                                        "h:i a": "G:i",
                                        "h:m:s m/d/Y": "d/m/Y H:i:s",
                                        "j": "j",
                                        "l F d, Y": "j F Y",
                                        "l g:ia": "l G:ia",
                                        "l, F d, Y": "j F, Y",
                                        "l, F j": "j F",
                                        "l, F j, Y": "j F Y",
                                        "l, F jS": "j F",
                                        "l, F jS, g:ia": "j F Y G:i",
                                        "l, M j": "j F",
                                        "l, M j, Y": "j F Y",
                                        "l, M j, Y g:ia": "j F Y G:i",
                                        "M d": "j F",
                                        "M d, Y": "j F Y",
                                        "M d, Y g:ia": "j F Y G:i",
                                        "M d, Y ga": "j F Y G",
                                        "M j": "j F",
                                        "M j, Y": "j F Y",
                                        "M j, Y g:i A": "j F Y G:i",
                                        "M j, Y g:ia": "j F Y G:i",
                                        "M jS, g:ia": "j F G:i",
                                        "M Y": "F Y",
                                        "M y": "j F",
                                        "m-d-y": "d/m/Y",
                                        "M. d": "j F",
                                        "M. d, Y": "j F Y",
                                        "j F Y": "j F Y",
                                        "m.d.y": "d/m/Y",
                                        "m/d": "d/m",
                                        "m/d/Y": "d/m/Y",
                                        "m/d/y": "d/m/Y",
                                        "m/d/Y g:ia": "d/m/Y H:i",
                                        "m/d/y H:i:s": "d/m/Y H:i:s",
                                        "m/d/Y h:m": "d/m/Y H:i:s",
                                        "n": "d/m",
                                        "n/j": "d/m",
                                        "n/j, g:ia": "d/m/Y H:i",
                                        "n/j/y": "d/m/Y",
                                        "Y": "Y",
                                        "Y-m-d": "d/m/Y",
                                        "Y/m/d": "d/m/Y",
                                        "y/m/d": "d/m/Y"
                                    },
                                    "ordinalSuffixes": {
                                        "1": "Ngày 1",
                                        "2": "Ngày 2",
                                        "3": "Ngày 3",
                                        "4": "Ngày 4",
                                        "5": "Ngày 5",
                                        "6": "Ngày 6",
                                        "7": "Ngày 7",
                                        "8": "Ngày 8",
                                        "9": "Ngày 9",
                                        "10": "Ngày 10",
                                        "11": "Ngày 11",
                                        "12": "Ngày 12",
                                        "13": "Ngày 13",
                                        "14": "Ngày 14",
                                        "15": "Ngày 15",
                                        "16": "Ngày 16",
                                        "17": "Ngày 17",
                                        "18": "Ngày 18",
                                        "19": "Ngày 19",
                                        "20": "Ngày 20",
                                        "21": "Ngày 21",
                                        "22": "Ngày 22",
                                        "23": "Ngày 23",
                                        "24": "Ngày 24",
                                        "25": "Ngày 25",
                                        "26": "Ngày 26",
                                        "27": "Ngày 27",
                                        "28": "Ngày 28",
                                        "29": "Ngày 29",
                                        "30": "Ngày 30",
                                        "31": "Ngày 31"
                                    }
                                },
                                165
                            ],
                            [
                                "CometCustomKeyCommands",
                                [],
                                {
                                    "customCommands": {},
                                    "areSingleKeysDisabled": null,
                                    "modifiedKeyboardShortcutsPreference": 4
                                },
                                4521
                            ],
                            [
                                "cr:7610",
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
                                "MentionsCommonWordsBlocklist",
                                [],
                                {
                                    "wordList": [
                                        "100",
                                        "Bac",
                                        "Ban",
                                        "Bác",
                                        "Bên",
                                        "Bạ",
                                        "Cam",
                                        "Cho",
                                        "Chu",
                                        "Chuc",
                                        "Chú",
                                        "Chúc",
                                        "Con",
                                        "Cua",
                                        "Cò",
                                        "Gio",
                                        "HCM",
                                        "Hâ",
                                        "Không",
                                        "Lai",
                                        "May",
                                        "Moi",
                                        "Mua",
                                        "NAM",
                                        "Nam",
                                        "Nho",
                                        "Noi",
                                        "PHA",
                                        "Phậ",
                                        "Phật",
                                        "Sao",
                                        "Thế",
                                        "Xin",
                                        "Xinh",
                                        "Yêu",
                                        "\\N",
                                        "bang",
                                        "banh",
                                        "binh",
                                        "biêt",
                                        "biế",
                                        "biển",
                                        "bong",
                                        "buon",
                                        "buôn",
                                        "bình",
                                        "bông",
                                        "cach",
                                        "cang",
                                        "canh",
                                        "chau",
                                        "chay",
                                        "chec",
                                        "check",
                                        "chia",
                                        "chie",
                                        "chinh",
                                        "chiên",
                                        "chiêu",
                                        "chiế",
                                        "chua",
                                        "chuc",
                                        "chung",
                                        "chuo",
                                        "chuy",
                                        "chuye",
                                        "chuyên",
                                        "chuân",
                                        "chân",
                                        "chí",
                                        "chúc",
                                        "chơ",
                                        "chưa",
                                        "chắc",
                                        "chốt",
                                        "cong",
                                        "cung",
                                        "cuoi",
                                        "công",
                                        "cươi",
                                        "cườ",
                                        "cả",
                                        "dang",
                                        "diệ",
                                        "doanh",
                                        "dong",
                                        "dung",
                                        "duoc",
                                        "dịch",
                                        "dụng",
                                        "giau",
                                        "gioi",
                                        "giúp",
                                        "giỏi",
                                        "hang",
                                        "hanh",
                                        "hinh",
                                        "hiên",
                                        "hàng",
                                        "hông",
                                        "iPO5",
                                        "khac",
                                        "khao",
                                        "khoa",
                                        "khoe",
                                        "khoi",
                                        "khong",
                                        "khá",
                                        "khác",
                                        "khôn",
                                        "không",
                                        "khỏe",
                                        "kinh",
                                        "kiêm",
                                        "kiế",
                                        "lang",
                                        "lich",
                                        "lien",
                                        "liên",
                                        "luon",
                                        "luong",
                                        "luôn",
                                        "lương",
                                        "mang",
                                        "manh",
                                        "minh",
                                        "miên",
                                        "mung",
                                        "muốn",
                                        "mình",
                                        "mư",
                                        "mưng",
                                        "mạ",
                                        "mừ",
                                        "mừng",
                                        "nang",
                                        "ngan",
                                        "ngay",
                                        "nghe",
                                        "nghie",
                                        "nghiêm",
                                        "nghiệ",
                                        "ngoa",
                                        "ngoai",
                                        "ngoan",
                                        "ngon",
                                        "nguo",
                                        "nguoi",
                                        "ngươ",
                                        "ngươi",
                                        "ngườ",
                                        "nhan",
                                        "nhanh",
                                        "nhat",
                                        "nhie",
                                        "nhin",
                                        "nhiê",
                                        "nhiên",
                                        "nhiêu",
                                        "nhiề",
                                        "nhân",
                                        "nhât",
                                        "nhìn",
                                        "nhóm",
                                        "nhăn",
                                        "nhưng",
                                        "nhấ",
                                        "nhậ",
                                        "nhập",
                                        "nhắn",
                                        "nhữn",
                                        "năng",
                                        "nươc",
                                        "nướ",
                                        "nước",
                                        "phon",
                                        "phong",
                                        "phuc",
                                        "phòng",
                                        "phải",
                                        "phậ",
                                        "phật",
                                        "quan",
                                        "quay",
                                        "quân",
                                        "sales",
                                        "sang",
                                        "ship",
                                        "shop",
                                        "sinh",
                                        "siêu",
                                        "sá",
                                        "sách",
                                        "số",
                                        "tang",
                                        "thai",
                                        "thang",
                                        "that",
                                        "thay",
                                        "them",
                                        "thich",
                                        "thie",
                                        "thoa",
                                        "thoai",
                                        "thoi",
                                        "thong",
                                        "thoáng",
                                        "thua",
                                        "thuon",
                                        "thuậ",
                                        "tháng",
                                        "thây",
                                        "thông",
                                        "thù",
                                        "thú",
                                        "thăn",
                                        "thăng",
                                        "thơm",
                                        "thưc",
                                        "thươn",
                                        "thầ",
                                        "thầy",
                                        "thậ",
                                        "thị",
                                        "thờ",
                                        "thời",
                                        "tien",
                                        "tinh",
                                        "tiế",
                                        "tiếp",
                                        "tiề",
                                        "toàn",
                                        "trie",
                                        "triệ",
                                        "trong",
                                        "truo",
                                        "trên",
                                        "trăn",
                                        "trươn",
                                        "trước",
                                        "trườ",
                                        "trực",
                                        "tuoi",
                                        "tuong",
                                        "tuye",
                                        "tuyê",
                                        "tuyên",
                                        "tuyể",
                                        "tuyển",
                                        "tì",
                                        "tươi",
                                        "tương",
                                        "tỉnh",
                                        "uông",
                                        "vang",
                                        "viên",
                                        "việ",
                                        "việc",
                                        "và",
                                        "vàng",
                                        "vâng",
                                        "xinh",
                                        "xong",
                                        "Đep",
                                        "Đẹp",
                                        "đang",
                                        "đinh",
                                        "đoan",
                                        "đong",
                                        "đá",
                                        "đì",
                                        "đình",
                                        "đông",
                                        "đồ",
                                        "độ"
                                    ]
                                },
                                6179
                            ],
                            [
                                "FbtQTOverrides",
                                [],
                                {
                                    "overrides": {
                                        "1_18f812b78098cc74bdf3dae35c973a2b": "Lập kế hoạch",
                                        "1_d87c336993f139af454adef746d7dce7": "Lập kế hoạch",
                                        "1_1ca9398c63ded1a46597aacc20828eb6": "{name} đã mời bạn tham gia kênh phát sóng {chat-name}.",
                                        "1_8a7b2f403c89955c76b99fbe86271991": "Đã mời bạn tham gia kênh phát sóng của họ: {chat-name}",
                                        "1_e69543b6eefac4e0d8288108ca5a83a4": "{creator} đã mời bạn tham gia kênh phát sóng của họ: {channel-name}.",
                                        "1_367ea8e1cb288c8cfe79e1dd1a7e54ce": "Đăng",
                                        "1_c65eb25cec72eb481713a2e7ed0b982b": "Đăng",
                                        "1_a4eb97b77f646af45144f2151b306ba0": "Đăng",
                                        "1_4ccfe710654643c123892ded5ed2a3fb": "Hình vẽ"
                                    }
                                },
                                551
                            ],
                            [
                                "AnalyticsCoreData",
                                [],
                                {
                                    "device_id": "$^|AcbYzxq461FyQY9klpBaW5-JJU18rC3pqkpF8jaDAtE7lFItyIr2JmKsVmMcEyKJ-mvxbYOFK8AvYZF5KrI0rSZsVyjeAes|fd.AcaYKn3XwASZ5ieTBGx3JfJER_i9-WopjVqD4GQkZYYP8frWKynlm40-EleyvjCs040mmonei_1fj9c4Y66OrMDI",
                                    "app_id": "2220391788200892",
                                    "enable_bladerunner": true,
                                    "enable_ack": true,
                                    "push_phase": "C3",
                                    "enable_observer": false,
                                    "enable_cmcd_observer": false,
                                    "enable_dataloss_timer": false,
                                    "enable_fallback_for_br": true,
                                    "queue_activation_experiment": false,
                                    "max_delay_br_queue": 60000,
                                    "max_delay_br_queue_immediate": 3,
                                    "max_delay_br_init_not_complete": 3000,
                                    "consents": {},
                                    "app_universe": 1,
                                    "br_stateful_migration_on": true,
                                    "enable_non_fb_br_stateless_by_default": false,
                                    "use_falco_as_mutex_key": false,
                                    "identity": {
                                        "fbIdentity": {
                                            "actorId": "61557504676830",
                                            "accountId": "61557504676830"
                                        },
                                        "claim": "hmac.AR2YHH-4FFIH441ocD0wgVW7VyFj4fmG6soLU4eX3YSsqPE8"
                                    },
                                    "state_for_br": "fase.AcZ4vg2Mbl_qfClyl84Kxzi_1eHJQjaPsFSa-7_dkg3m6PgqwhY955XLjhrPpJwqKGY6Emn-qSSDlrdxRYObtTKZAZBdJ-iG0AVO98skhrM5n_HsZ1Qfq_oOQoDtjfIONK9ev1im0114Ax0Afz6GLzllKmmLIAjtvxH-l0VSvxb8vT3YVwTTQOqzG5sKyQzsdwdSCt39GTuNeSdu9GMnQ7Ep9HzSU6xKXwRG1rOOtmgySnd8qfPlx2nrxp2Lye23EyrDjNzD3VEDxL7ingbBCYCKtGaHq6agySiH_nhrdL53M5AipuQoXHnGQkn8nwLLlIKyqQUrudHgSEpzL_wQBHHaJtHa4E4vrdTlEe7dbt2XJMpR1rwvit0otWMo2EGQ6uqkrdEcCtm53rPyJoLJ5VP6pNzE2pXeeHkzeCvGhgitoC2AedoBOjP_aHE4NxLPKYlZbh2Disfcnx1eylCGgmRBlfoXuWZtjMxeWqhOFWNf-IHMxBqT0NS-VHs6adRd47wy6TxE6Ul3UQVSqK3Fc-vNhlQUzQzcQ3BviP422c6u6VbnarOmdaZerLTfeudIpIds4QvLKCEYHx9O4dVt46mHwHtQmR3CdvtHn9bEotb3KRgxScc16IP1xczCfqwrvCz5Fc2uu6jdAWDNFrBZwx2ly0oRikQ1gZNx28HKGRVZWGm4IhOxxcJAK4So3ADAxqQMmRUjLY0qVKWjDMXfSMw_95HpvLNCLOYcXyXdSQv0TYDHmyLbxmJf6KnfaLE5Zd6tnPbDhJ6VJcbibFmrrj7b3vymKim3U69twj5vdwelhg5p2NmlkXIMffOHgo9Ac-9yzr1Wi9wOrPxzszaxEXRlA-y9_jBQerewg3BRH2u4HUW7zlN-EGEd4UKtTlaF53ShOKIfAh4ZXZvqZhG5eMwy-JKpYItCsP5kwfT0VkQgqTrsCT6eWa9S9A3Ht-odpRFfeY7FCrJxay_c360dP3NyCOSG9T2TH7PN2k8zrqdDuqiDrCUO2x2YVSuc8Q5VfbNZMC2FewB-If6pTdPQUOHSNkmGXC-mkLj-qNXfGGEd1H7MqBQR0hzDvwUjpByVy0VmODqLKXE23Pmc2rSS3qdncSdTiMw8972cwtVcPTg9UjzSw9f1NbdEnlZ4HT3DLPe3wzcCfoQ_7wREKGC2B4m3DAWdSpB-Z3edwUo4EZGglnS2keAvz8OHCJmMdoJwQSCaR43BcKuAf_ZoN_87tBskrXUWqiBCiZcYA2fm5zJryViclPE8qE-Ilvv2IMnPYqDgkfwGQ1CnfSe7ydIiZ65G-IvoggqKj6v-jcU-wsatX5jO4_6DpsxnyigDQ4Ey2bYV1CuGrLENaQr4LNyqrFiMIXzHK7CE40KWoGfjVg8fyIJZQj2Q35vj4DnTcdbRiQzKDRxsynkj5u_8JLl_EYTdM1KwegxBYNdcQ2GqRM2zj09gZmHFSroZ_R9KQQI326cF8C--rxzax6z2PYjBRhEj6g0mTyi1c3vD5bNETpls1BJtdy_pYUmB7grtdxu6uT_CUjvX_CP07d-CqYrDe4h0Re36fuJRFM2JMR3YfwyEtbnryI8zr-qfKMDKxdqu48FibCZiU6x1aNzzsuh7ePP-ZYWITl0c-ClESqITTHJdxQDK2FzfA0j3ThFkB1fyTYOZlaN1-2FNipvPtSypN7hoX8I-X4vqUZ8QPQ73nojiqcWvWnRFEfYM_5vTg5T4Kykg6nFnDN2ageKCrPuZslUX3Wa9LXPknCJ9V65OeZlvsuFPRVdww9po9x7qu1bdnIQJI2mQSI_kop6bFJWKAtxPTwA0QTfAPpl0YeOR8oYy1BY1szfokl2vWPExY2rQ7HzPljJdjtBO0hetazc0pMjDf1TDhjn2dY9rXG5EGNIxKcf6AwZ0LkEVDXV69vfvX3qRpVqUS5NZmwTHgvx1y1Hh7tWKBS3hxBbp4iT82D8hZI_CchL5BZiF8vcBRaBQ4LPwMrncmAbQno01G2qixrfDBgAaAWeHeEPsrtkVpafWwtt6cBJrYwuoukZsq__l1TfXKLHUHaBFyk_Ar07_3YnQlm7W4fR4gnZXNHP-kyklZrn6Kxl0QJmYO0WUqyTAHTPuF58ePZEJaUZ3orkqJK1q1rK4JK7o7Gfzy74tH2EQPairHDZ16FA_pijhx_xYIC5dsRf_S-P6XhZjasZ5BH7dLxkUfzybV8d4rA0xb3sAdEtdPaL9d4fvQrnH7RD3gUR5iyv-8avNpJqxo_NUiEYutpV_LQ-xulYoEVxCPKnDwIDIrgK6XlqSyMMEjpRtYLFHRTRPHYyKpov9Gv9FlaLn_UF8f0-V_9PZhc5qfEv4DXFz7u6bYXkyHD0j1WakryT7d-vUfw113sdHTgZtFrP6hEMb0gpMpyzHcrVB2OAtlElvGPUi8Obiv1PhC1m2ACPCIULt51YGaXXYP8goOGfMtezTzW0CJhCIwZJAwlOFdeGJ8OaQnk3UUzb6FivBnyRpzNghFiNdsXlB7UY96FfINAeZNbNvvx_EfaHl4wsAi_OdFTtP-Q3QGCHcKi-3yaK-xEeJ0jtP9eReOSLlmPOglJcYoa_T9JkDp78aR0qHfEmuxfhdWItXZivi1ivChxlv2pM3ldPD6C0VbhqJsQ-3cAgDShm18jzRiXPZFvRj8nCGi3xje8p7wa6nvhREQoECuwHhAYj0FfQRN1hoJlIaT7tltMYapNWS7O2IM-KvNyXzbv0WIlleifosNI2pZAhfZ3rmzr10tdzzpOh4m9SWRuLCqlflPXLduT-U6b8hjI2dxygucyKLvWjNMStdoHuA6YVMFgz-Kk8Nrjp8hvc6j1KHGarnD1vol6hvuTO4nuVgLXHDXQJHltURj9LFji5TyYUFKDtF4IjNXREuf-eOOPDF9mBDp3hsLO-Cga2W2g6HHAwp2hjQ1WXwHd360ppVFUWTGH3JE7cLwK5WlVGw8vPY8_Zz6qwG7hU-hePzhvd6aC6KyKTU_YMSxlQtykGKWYckCiYV9X6kwOZrW_OPQK0tyBfUtd8DHUnT0URQ1Q-MPa1hbtzqtmLU4-5XyO65Foivm9HrNIXIn8UH8bR3jkBIorqnvCocvocfhditnA_C7AvjoefjDEir_a9G-N1X5k5l55joMDwV4ymbAiuWZeTAz_y_owHzYdcpdOrE7WeHbhLYWJgdmyQobj29NjwCSO5RPwQ6RV26FN22GqoToiBM-rGGsXhf-UPWeh6qy_ikx5gvL80otv9s_hBUurD_gYuE8CjvZY3xJwwaTMTqccwyGmrubXvV0JPtqI6ZQF7PorXd5mm6JdyZrHNuEgIHd4no7TLEEk-hWRT_LYmK9E2OPwvEzeogXekGp4lMpmTRlW07dTuodO9cq_3ADa4ZGjBdadz-gFs-fnnohN52flXgmwx2C_K6NhHVYB6d1Q3yi6BMl_uP9pcXYSimP5VSVqF_imFTniUc5Rm2EdcmE4t5dTHr_54XzD438ULnKWoxMJ0IbYKhZSgCUOdkgvpX2ZZjUX_MWWxsfc8Oz0fz2BoJKFjFsmSsZBOWQyvJxngUrwfiR_j4E7yGLzWRI_rBXPvEa_fIGX6AoUzspr1wx_nhv5zwre0QUvXaUWrIDUuKpBiVBo2KE3GYiOwMhHL2hlsgHY4Jzab1ynSQoCmGw7O6SGI_yTqfljxaE3NcNsdLBrTfuS8owQZsGPuuPZ5YMUVk1yxnROr8XRNFDGNRfMCnaQPPFis9aVRMKaqXNAg1Wpxsd3Uo3R5yjRJsPP6ouUacCIodseLI6UYQmju4rP_38pZtl1mGrRDKK4wd5_bLarehRRRSj7xg0cQIPsIXDvfNhqNhy4h0b3Bg0E-rZz-rzCg96x6igPp-ZWJrZgHjFXjpfri7N3nSZBACPmqnUmKDgsUzpm0lAF3UnB_kl3a_zEdJgxDrLYR9DluXFZEMN8p9aCM1cxQPnM1JiZRtRoWmgA2wJsgN9t-1KEdC8Q5XeK5pzvTmWqlbNP74slZwjvUDPfSAtDT1GnYfq4klcSqbmr0ReKZBrLPP5m-oj-3i6LAlrieczGaKiXyaEl9YFc3nlle1xCADz1000PLwNX0VBq04QJSZtyb0STtggM9PVTZQr5RwkXS4BBs3dqzX4p6Pv7z37u0VG3h9P13NK4wyXNEnpmV65B2qoxOktyBbe3_7drXIbYLeU-fjSGwS_IGZnuUVyQgWRX15KTcWbHyzF0uaYTPgNZeEX1ja80Y1V8RD2MC-ENklF7X18EJoJZ_KXbquXwK-hzbyjNMnd20VcrOARJgD3RJ_iz5sNL8F8IGrCJYRlAcEvdBxzOeRG3beHOmaAMBucGaV9Re0aDv6BWc4qYXfqHQbfo0AJfRW_mkhIbfJ4JQMPqUnV8IcvdBD14FR8q3Oy0Bjh3eFrxRIznxQevb5TEhmN_UXw5kaIOSzcDtIp2K8JcssOkvWtmtyat1T1oohn7x0Zvkh_tcK85DZ8kf9Nw7FoWA-1pAhgkbQVEXZ_URXQeL6oU0w3GJIyiWOEv7EpNNcEYD6O75o78wPZ4lWBEi27kYcfpTAnPRcBs2XeH6MQyoacEO_0tOKyHBKU3HfEXSX_6BUU6ylJzrEYZkQtvJV-1PzhdBPu_eUFdr_df44ihrPc0mABy3qNU3s7DmGK8yrViKZqT9UpUIag_60WhvpNNWXJFWCNI6OvHTs7aGsR_arBUgqAqL1Mdg0OwvLiEVN7nkOBIWT6qFHkJCr3ZuylKc_h5DwPTcdGnqoML3FGUtsnH_--lNK-3JjxCA2X0GW4lChMbH0J5-VSXHSEJU5CMFBqfMtyLHdNTkV00tDnPdKvnqWWpuALIZ0hVnDIrwsKY3CluSHKAAWG-LssGW68nS9Q5eQrb9cZnBwMsveQ30ditFSHp1wO7CDL3jp4K9puza4Q8V5LO4JIi9LJdNxVLEoTSZKf42krKJUUqKwHKnOaVMCqmUGZJWCCMguCOkGgmLSEALgoENevbN34oez05LK5VWHiNnD5IfPAdpfNZslqIRPZLWvVkMZ_kIFW-A6EbdyDOSxCEM8QLV50CeuADvTRo33m7v9-U5MZl_U4iCkxo4Ijv1_ph63jFzqKgo5tlLch2DgHFgNyM3DsLQjYpUfPMiW5Y9K4yQUKsLMxdz6pEDaATODFT4MOTWj_lUZCRcVLzrLHW8FXLf5d_JLU-PDCarxFAyait9X6P5jyUPT34qRrvl8pXESXMCL5TA2EGuYC8_ieLHwMSI4s1bFKhaDu1YWmg3ijBGwYLeXeMYNtPxnkDpyAt5g7wocP1aUH_Eu7NTRSN8neIZs7z2a2N8VZa_97c3-OV_6SRA_owd1JbIZdqdZR7rNBrHvpLqtjAmM3BDeK1QlSqvZrQDjppCdiFXAADlBAA",
                                    "stateful_events_list_for_br": [
                                        "comet_metrics_viewable_impression",
                                        "web_time_spent_bit_array",
                                        "web_time_spent_navigation",
                                        "cloud_gaming_events",
                                        "cloud_gaming_session_event"
                                    ]
                                },
                                5237
                            ],
                            [
                                "GetAsyncParamsExtraData",
                                [],
                                {
                                    "extra_data": {}
                                },
                                7511
                            ],
                            [
                                "MqttWebConfig",
                                [],
                                {
                                    "fbid": "61557504676830",
                                    "appID": 219994525426954,
                                    "endpoint": "wss://edge-chat.facebook.com/chat?region=prn",
                                    "pollingEndpoint": "https://edge-chat.facebook.com/mqtt/pull?region=prn",
                                    "subscribedTopics": [],
                                    "capabilities": 10,
                                    "clientCapabilities": 3,
                                    "chatVisibility": true,
                                    "hostNameOverride": ""
                                },
                                3790
                            ],
                            [
                                "LinkshimHandlerConfig",
                                [],
                                {
                                    "supports_meta_referrer": true,
                                    "default_meta_referrer_policy": "origin-when-crossorigin",
                                    "switched_meta_referrer_policy": "origin",
                                    "non_linkshim_lnfb_mode": null,
                                    "link_react_default_hash": "AT2CEKH8GFlqr835r8Xndit0zSlqs9eM0Vlc8Nh6cCe-09rKUI8fZ3NbFRcACQXJHl9UqjXpK1yUBY_RG7l6Nu7hovYmLJtj3dX2MfvbL2b2YRZ-V3fi3v2cAZcTnH5KA7iyqVRgxg",
                                    "untrusted_link_default_hash": "AT0KGcZh6L3yqWxuk1nrbkbQGGOyRI50oTP9kp2JLB3-ntqqNVTtJzdaGdoElT1c2iMzZe1j43oPzgiUuYP9LoydaS8bSBQiFN754QqmLYgLoAZhCdD1WRCn0NbllyfH6UnD9VgNRA",
                                    "linkshim_host": "l.facebook.com",
                                    "linkshim_path": "/l.php",
                                    "linkshim_enc_param": "h",
                                    "linkshim_url_param": "u",
                                    "use_rel_no_opener": true,
                                    "use_rel_no_referrer": true,
                                    "always_use_https": true,
                                    "onion_always_shim": true,
                                    "middle_click_requires_event": true,
                                    "www_safe_js_mode": "asynclazy",
                                    "m_safe_js_mode": "MLynx_asynclazy",
                                    "ghl_param_link_shim": false,
                                    "click_ids": [
                                        "IwAR1QzjBvKPyectG53ApaS7yA9sH-OtCnG-23HgRVgCpobVB-dizhg--O4HI_aem_Afu6hft1GIvpERcSf9kNw16JG5wsNZrd62j97zzoodRtQnBXNZG89_LfTuyNOD0SYcHEI3hFO121R_VbSFH_BKFQ",
                                        "IwAR2fCdtolURwbkg_4HSZM3IfAq-uUamZutDbcA0k9_vEbEjo-Ml6mmhDhdA_aem_AftTz9eloa4pf3H0ftRmzOtIaYp5vPMfmy0UHRf1KqV47fj9EkJlxm2uJAYUqieK-byDr-045e5aWFBGoGHZoMWI",
                                        "IwAR3n5_vHqFdUqrqweNQnMvmK9EsJkyrowO4fGTGmAlTLP-pPqyvLGwhRG0M_aem_AfuEWP7B8X2zWHKSdRILzeNH3_qIBkLJmrM5O8dKpRFybrTGfnPtemlqjtou_NFMnX_fKOXuwzCUYA0jGWCytHg5",
                                        "IwAR0or4TxopRF1xQidX8tYs30vt_hLoBIoOo956T2XDb3gyTTO251uJ5awi4_aem_Afut1Cg-40r4vuU8fbbxTMW-gu_9KPcT3XjNBhBM8bJXNJTpXDXFzMBnWh6zjW5rPoJ1r9Mr09VuKj_9e9wX1aY6",
                                        "IwAR1FW5iN9nqNOq_p3WSr1yE-bVopss-SSGvuukK9hfDsOBoMeC8XgrTaDJQ_aem_Afv5grkrWXs5iK3M4UP1Ji8mb1IllIA2pkFGZdytyQpG6T-HIvXIw8oBnDsHCVS49WsAXmyCEC9Nzz9VDqKQFxrx",
                                        "IwAR2aUeyqAtUcygHTpwaBLBaU86it2itArBgdVgxumlfafLVRSK1vQqXEfYo_aem_AfvnxhDpb33ocwqxHRlDqWQVV2o0Kc7E6BSWzFuXCNTXrjjRpdabIh-uhwX6pWB6S270_KSPi0uqZqO9QTWBJAHk",
                                        "IwAR2k048VT__5QFerNMLGvsHHqjHJwY2MhhNvWUT11Ps6GmhQBbBBDKc8m94_aem_AfuqJArgby0vF2CQjxFft0XpFz0SuOoM3yiw7gErwECisO7t7mM_2URpQAkIzLoMnAmQOtUTlWdbWs2u5TGiWgWd",
                                        "IwAR2eXi7g6x1pAvpuDeaL6Rg_yzfiaka5lDM5JcDe3VpJYMMdSPGhJ3RSAD4_aem_AfuT1Y9v-7RRiEp160g0gA8Bgm57_0zc6PhbyuVEyJrmQCllzlzs5p_ISjQ1XZV9r_qd9TnmP12D3C0tXI3yFyIo",
                                        "IwAR1cHjqx9nT7baJfWpCJ7P-tjOpCCpY9HfLoAkhv772ywWyfkGOgMikK9Hk_aem_AfuSdvQ9W5sAHKxV7xKbewIs86x4uMM98mx4ce3G4PHksPMrLrag0sr17-_24H1d8wm3murO2TgdtCi6SS0VNwhV",
                                        "IwAR0BnopXI-dDVb9kSAxEkG01U5ij1dnZENWPSDv66QbIzOM4xRPJE80rzFg_aem_Aftj_YqDk421nhocPfi1Wb35yl5kHom-jWAq3FAdacseDPSx_eSHDKSlo3-JEwxB3kE_UBqiZKUpT4y0QPFvER1u",
                                        "IwAR0IW0tq_BFbFEmHDtBJKhwe6_HyZlIL8-V3pySJkuLHjJUF8QVrmA_xwDk_aem_AfsK3ceM8F04dTeJilR2EahNcpQkEuGUvgGjW7EYX2CR-smJrWXUBEsk1M4dukQi7ZWEAa8fxkzyllclzzSX9Xjk",
                                        "IwAR0Me8XVXwxZRGW9esGgacwQ5SnaAdHjrdUUIcV5UtY3THnHsUHUR1igsVk_aem_AftXixFeZZgYMXb-Tl_0-aytIrdACBrjhcUprTp-dK3RzrNflZirO-19RD9zs-bqhTyWwqC8EwS7lIOZTGPL9xCI",
                                        "IwAR0lrayDPSHZA4DW0MYJ6HCTRDX8lUiuvOnrBxPYY31gYc-RJH-WMoST05o_aem_AftgQIfgEz2rE-6fr8xEgIOefr16kL_0gJtjqYKyTgrUCtib9vygPh7rwbJ9gc26CmT6WrHmGnngQPANaAOndC6R",
                                        "IwAR2MIoWQmgPC6oc_DrQKZ2_5S4Jd-t4CO21UjzCRaVpmGAz-dEZ3lpYalB8_aem_Afv6mp7k8MCju0cQOuSest_niGnpvWA8_eqX-v2MNVp_2cMcUDpw6oetzIskkP4glWNbD1hS5dveZ3Pga_41OE9V",
                                        "IwAR3OQlpEX_d6MPBLA3_FMhxEWVSOooerW-jhrWECgeH10ZSh9gjmD3cE_-8_aem_Afs0qCCT48Q0XcY3zgB1yVEZjPrYKhLaVTcWJXiVsnif74WtLf8vIxclOu_eJrsFx-1gqBClMk5nfrPs6-E9MuQs",
                                        "IwAR00jPb63wmxrPvTXc26feHqs0aaIK8tANJwR3Jz2sJWFmycdXK3vPwFe-o_aem_AfulCcB-4QC0JtWMywOeym_tGSeN2e3_7wLUFIUo_M7kSyux6o2med6TChOLtKAw8_O20oPib_1LiNkKB3W3l18e",
                                        "IwAR3cpsAI2RHa_tOYU1VkTF1ZLu41DDv9VtRK38LQUPTu_IsmCI0wy7ewsfc_aem_Afv3uGIF8PWhu66I65Af8fhM94mC-4l1I7OvLp6SowHYb_1Lbbh4AZboDpMthJTiF98n443Q1LIvwcuWWkZF0J2w",
                                        "IwAR0_3rRHJnTXvtGNKJ8lbg5MZRQrCmI_nogfFFDZLnNJRTLgamwSWZ8oa7Q_aem_AfsRzbEX0fI8e69b6UbOioTewNLFtGS5WDmbTtFTJNT6naPmQLSbOidcUYhLoZgntg2XD0Itdoy6BRabmnlFnU36",
                                        "IwAR3v-LtbpY9jmXfEWk8hYLzoqRseKf3SVgQ4wQ_4DIi7vbiMnuVPMccE6cs_aem_Afs2_GNKC30pw-gDycqBPLJ5e4TxxEPGXwBlVCYf-dfd4PG54utHEcunjRrsnM2v9jM7AlqACVpp4aX4fI62df-r",
                                        "IwAR07CaO8GCBj4_9vVfHyuUdNR23hbvBAWu660eW8G2AaPViopLm5CUSf0qU_aem_Aft6-IJyb2BO5NUhA6zTwwQBMwy0zUnPM8WqK249EbmJxs8Bb96d8aLU8S5myuVVqA709s0sTXuCKI_W-D-HxBh9",
                                        "IwAR1Y0CjEuUehy04ZvT6yUToCH6_crrBKxaQBr51KnKwjnorkb4z-4DGvFwo_aem_Afu1bZyYrNHB0xCgHWI8pFwUeq_HiQLkzO1Wp8dmA73fmlcF7eOaklIHSZiL9Qfa7m_zhq2frm_8IQFtczR0zSpq",
                                        "IwAR2uZQbX6A37bfsDLeKXLNMvAVOFmGAZdte8Gv4i3n1Vb01bZ_3e-Dm1Gzs_aem_AfssrI-CP7UdyADIEc2RV-AnwnWsV5DWz29lxcqnCffuqnG5GB98loIFAOhcbL_eVDGrKNwlkIpwoQ3NgFQHuslR",
                                        "IwAR1gVmix2WuLotYneaGwNoW0Q71EZtH3bluEFw49UD8pnaavYr4fQFaSe_A_aem_AfsjBYffZCtjs8Jr13hXHkJ-TwNiiKUXsv7otdzz9h5ixWSTxjrI4TEQO6SGhlcji2_OIvKh61eXT7k9skQlZ5ww",
                                        "IwAR31IWQiBf6_sQGZnZTgJrDU6kIdIzOci1mxtHwJPyzBqfyJgDM_7IncB2U_aem_Afv4fs7yNlG1wvUt3IdLbeL5uuKZMfhHQmOBcHaozfHapG2s8Tk9EEyHeE0SrbAzHzNBT2MshnTzELsVGJBfYshC",
                                        "IwAR1JDhTOwpt17rto9UON_paXwkA1SallHDkJ1r6FQa5k19ov4uiapfAYeD0_aem_AfuTLAC7bkrYBYI6PdLNOF09ctR3XX7--jDNLznkQO3VvLKLtXcpjQZ8_UHcDXsYQLLW6cqcKdV1yc2cyFOyeFFy",
                                        "IwAR0hXpvCcvEd9o_0VuG755jUvPe_Yx5vBMsSi7Kbtjtu5d3-Sc9mg5iXqMQ_aem_AfvCq8R6T7a_bNoZotu4eRaCJhjKGSFp8jXEwvl-JHghVgao3Tjxlo8uF6RIXjyjWl0gn6hu3MF0sfTP6hOZcjF9",
                                        "IwAR1wAxkjAfjCTT0yUAdMvJrRgNZtmIXjWnNTVcTxtTROFaUXtasHgJ6iWq8_aem_Afvzr8zFKULaHF0RR3DPPw7SVwxzAfB3jBC351kNi-cs0J4c2L_hjh80aGSmz8UalQbW1oMKD37ql9a5mn1GtUt0",
                                        "IwAR2B1dNs5y7cEXmAt3UMY2HELqqwZDPAob324YqwLkjYf3JSnYdJULJaH1c_aem_Afv46VnONJOlvBPmpA-fYukN_wtmvci0gFdws2yk_xp7VXuAJcFaumH-IzJTTnN55U9bXfb4X8Pc35jagKBFbeEV",
                                        "IwAR3zoDca7xxhD0n3PWULAS1DzfvGvcGe9MXMY4eYcQ79Gw4gAKsaWKbcTek_aem_AfuiEfed52eQEAHG9BcMMiRVdp1GGihECpR4yEWORQEGDoKMble6XNLtVTEz5vmFb6j2xHlvoLCyDyep6SPhcb87",
                                        "IwAR2sFvmIM3DK03qsWtTqpviZlNx4u8bPYcWWb5tYWvE4v28sCLT2eOov5os_aem_AftmQ9KtB4Xpb8v8se7LpQbjvk32_Wv1rsy3DUGA7hLfH1VgTa2cTjJg9Idj5R3hHxvHWupsHVj5ZEcybAh8Ogsv",
                                        "IwAR2QinLw3GGlu0gjhRDM2YdeQAR_RcB_5nEZ0aBfFuEM7ztwRTPkhb5pcvI_aem_AfvxGgg53BJd4WjOEMV1UxmW4dGamPj-QN5TTxcwNDHJHuTVvg8o_uHZJEjm5G8l20OqvNNlkpYGwWlJ8ctfmHbt",
                                        "IwAR3LetIiWfMd1JUSD47HjM0gw9X2_4vMEyp5RaZMXhwLl_YQOcIqNTIzN38_aem_AfvFEOQrh0_OYe_Q90nTYV6Uuugjz7dDBjfS1iwNYh-Mm9Zdvd6WSJnEN4Jbea1bcjhra02TES5JssfQj9QW8tII",
                                        "IwAR0vl7-SZ5vMC2WWyHbObeKsoupAXrxIE6YyZFZxJKhwo0CaX54G88aSfaI_aem_Aft5XXHMY4v_e80oSKSuTFV13cMpYusipXiD7FiPXIlYEIwpxGXkprutPKsqbuezfcI36ErHomzQc045Sw7q8H6j",
                                        "IwAR2NfpV0KjHqelg3lIpUgZwuCAvj0rBwTVTj5QJ8SRzGzC29exA5m86UHE4_aem_AfvZCxOFAzR4Yr2eKubz3sbE1HaGELv67axgzXrcZuPWecG4FxeSLxn9cGuxlNnRWYlEg2MjfvyTORFy4zpDrIjV",
                                        "IwAR3Sd6uSd-rwIuMRF6n9odjp3rjbpXxeieWwZFTsWc9WBTRGYovRy0UNwh8_aem_AfvC-okwvXLG0d1FKhQWgrCWz3nehoLoGcS_-vk1uJ_VADOV4RDTKxLYeMzVy_4F3tiIl9LXeYbfr0Is0cK5TaZ2",
                                        "IwAR2LRLIa6VQIQGgdZZJa4C61nQF1sKdBpWM1FUdw1k-kQy_mqjz-aV1_JMY_aem_Afu23w7O3J83AGzqHkSjdytEnypFqkn257iNzmrMzHlQeN_ou7QzptkFklWqIYMV36hqEdh-_xx517cpGFavoSXL",
                                        "IwAR11OH7RjbzLPe26hFL_p7SZmdwKWBA4cMrBvRreGgIKxqUPuhAmEBeDvzU_aem_Afs2_uZ9rNkbd4MvltuOdajV070O7mPEaLdjZ18NQofZvHl77_EocQpuEb4ouvzRDSmirZLf1HCNIyZtOK3xtH67",
                                        "IwAR2ANmvYm9o5C_hPXqjFmwFPp_Vdl4I9D1AiiFWRKWGsZIzMfwzEFY00obc_aem_Afs9u38m-l5PLF_YDoXgUwe7uxFOMtas_jjG7oQj3JxzmAcarnK2CxJVOp6_0Czg1tFXCeor-Ml-MGn8uZPEjkqL",
                                        "IwAR2Nl5hjjUcq122AvguVvYXl0Rm3tC5D1eJs0JRzbYNpOxsk2xJtjSmOFGc_aem_AfsXr-aEGWKA18ETJn_4yIAJKPIsoqq_WM8HlsudNi5e2E8EM1-ZsDAvP4lK5q1USzjjJ7_lixLnyhw2BVFa5rdl",
                                        "IwAR3xj8bXF97deBLY9cIPsGrkwFqZT0sP0u0DU4V9WGIeunMC2jJNnUhMaA8_aem_Afv660A7UCJDRA2EsSeOSlho98bhJtznLY8l2tMMKvPsrC8Z_cEJIwA-JnmPksmyr0A63eleJdV3G6hVOazWQ_Yk",
                                        "IwAR2nEMLJ7c3WXVqC1zOBlDJsXI5bxw5JAIyX5dsIsVHn2UNa11wrdGHEG4k_aem_AftaE5a4KB2lBZsRChcvD5LmHjpyY_T2y1qWDQrvY78kERYiHhQRxS81LN8WayQoRT3jdubJpn3U3e7YwUE7HRE8",
                                        "IwAR1Nqh5NnYomdWU60keEZYNa4dtiyKXT2vstR9mF02IR69R5hmT6jBvKIy8_aem_Afu1xbQ3N0KPy7XXFtgphQDL6GHpbvG61dSXqSTFXhwk1dcDeUFGBiuywX6WeQaBYuARju__DZsw1uwXfhQzKvq6",
                                        "IwAR0KpUr6lm55EnjIePBFQzUe0xuizOY3a0aMs1G10FJXY_3ycxLJd8M2288_aem_AfsNkqW5NFmY2XlGfZm-X7lUShByLAaXHwHLcg_tfjgVSNljq21IgGUruTrxqG7HYyKJdyyo2RZU1IgxXLBquLG3",
                                        "IwAR1Yf5aCFDUl33DSFmx5_2QYFSBHPb4IRY-g8D19kuFEL5cVK8zLi1yqYYM_aem_AfuLEHTWSntXdmtatK9dxnVB2f7ffYfKnSf1oNgqxeWloz_A5WBV3Kbe29v29Edr7KUx2XylKWBt3uBV9Eg_D6O1",
                                        "IwAR0BvnHa9O6hjPWRH-_R6ny2k5FZd6hawXgwtco28h4PDFp-tSyX6AMXhmA_aem_AftmdshiP74e7JKYpRcUH6aDjfsdBby0mM651WtkHxIL1hZbf0Von67EfjSTSroKgzO155USdre19T6qNGWgw0OD",
                                        "IwAR0_WRPA8Gyf4ABTUwGYV_7Gd08xhkvsyQM4AR5NlTjnF6f0a7Xd-JyT10w_aem_Afv6OO_noqJDNvKww4S_RqBarB2LVEKSA_OwDmJmYht9ajsvGv6Nc7K6SAzwThmhRiu2GCg4P9J9i-W2-fnmucYj",
                                        "IwAR2K-a4IHVBhZEkUnh6RWq77V4c3LXo8EVJWwfBFKDRIVw_CDvmKMSLO4fo_aem_AfuqeqdbkPAaLkFdSxVxjlIPTCJ3VBu0JfcouMUQfcSjNzqKQP1EdOgUk5RVG7L1TKOQ-uc_-2qxQqKLZz-XjiEa",
                                        "IwAR181Vd8Jg5Mpi5sxlBYwz_rSXbsEcEzm-t3QBByg2gwjxurVHXwwFa66D8_aem_Afv6Hhddl1rQQKzNFyxSXqjUuXr2B48o0gO0MOuUukuNTE3zjUsrkIVwxnVJuXFQIC-JE0A4WW94VT0fBSDSD0nT",
                                        "IwAR2-9lWTYmm7Va_z3W1sUF8WnX7GJ5F2jA4qc0gH901qT5gyLCw2dzUvdro_aem_Afvacx2Zk_Qya-eSDrHcVcaHDxoEobF0TUAX8OfqvrrPZTumHeVQ9dg92oRwjsmZBuQCAJbebTkIYz2uICt8H6Rj",
                                        "IwAR2PVA_48L2WfU6MvHqOktvRGs1vugmtKvgLEPbvSsyRnd5lKVh6p6oN_AA_aem_Aft97H6Rbrvb7f3jR6E73URALq6TFqPMh9f0hhD0P0GFg0l2CFk3TaA3CVIxmPa8tOTC2G2Cfi3CrssmhgAkCDoZ"
                                    ],
                                    "is_linkshim_supported": true,
                                    "current_domain": "facebook.com",
                                    "blocklisted_domains": [
                                        "ad.doubleclick.net",
                                        "ads-encryption-url-example.com",
                                        "bs.serving-sys.com",
                                        "ad.atdmt.com",
                                        "adform.net",
                                        "ad13.adfarm1.adition.com",
                                        "ilovemyfreedoms.com",
                                        "secure.adnxs.com"
                                    ],
                                    "is_mobile_device": false
                                },
                                27
                            ],
                            [
                                "cr:7608",
                                [
                                    "MAWMIC"
                                ],
                                {
                                    "__rc": [
                                        "MAWMIC",
                                        "Aa3RoqbAIP0fZadExpuqqG7G7X6vOqK_RBvshUWUbzi2jW2ke8YMmr_rgApLkgayoSPlW1jFRKkrbpbA_ERh8ylUHEEhi6wowjyS5j86ipdT"
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:6045",
                                [
                                    "LSRelayEnvironmentConfig"
                                ],
                                {
                                    "__rc": [
                                        "LSRelayEnvironmentConfig",
                                        "Aa1rH5pKrq8pcRryiMf5G6Bn0gzgl4rM50GUnvNfnRxQ0QdRctIVvbMdZzIZ-vSzs56A8LznMMDCZ40zzgu8NKyNsv4c14_FPPuQ8vERsZwKUY2upp5dUT0AwH-xAWNGrZLFJEAr_KzsG8n43g"
                                    ]
                                },
                                -1
                            ],
                            [
                                "cr:5889",
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
                                "cr:2928",
                                [
                                    "CometLiveResolverStore"
                                ],
                                {
                                    "__rc": [
                                        "CometLiveResolverStore",
                                        null
                                    ]
                                },
                                -1
                            ]
                        ],
                        "require": [
                            [
                                "CometGenericCommentDisableNotice_commentDisableNotice$normalization.graphql"
                            ],
                            [
                                "CometGenericCommentDisableNotice.react"
                            ],
                            [
                                "cometUFIComposerGroupMentionsPlugin_plugin$normalization.graphql"
                            ],
                            [
                                "cometUFIComposerGroupMentionsPlugin"
                            ],
                            [
                                "cometUFIComposerAvatarPlugin_plugin$normalization.graphql"
                            ],
                            [
                                "cometUFIComposerAvatarPlugin"
                            ],
                            [
                                "cometUFIComposerHashtagPlugin_plugin$normalization.graphql"
                            ],
                            [
                                "cometUFIComposerHashtagPlugin"
                            ],
                            [
                                "cometUFIComposerEmojiPlugin_plugin$normalization.graphql"
                            ],
                            [
                                "cometUFIComposerEmojiPlugin"
                            ],
                            [
                                "cometUFIComposerMediaUploadPlugin_plugin$normalization.graphql"
                            ],
                            [
                                "cometUFIComposerMediaUploadPlugin"
                            ],
                            [
                                "cometUFIComposerGIFPlugin_plugin$normalization.graphql"
                            ],
                            [
                                "cometUFIComposerGIFPlugin"
                            ],
                            [
                                "cometUFIComposerStickersPlugin_next_plugin$normalization.graphql"
                            ],
                            [
                                "cometUFIComposerStickersPlugin.next"
                            ],
                            [
                                "cometUFIComposerEmoticonPlugin_plugin$normalization.graphql"
                            ],
                            [
                                "cometUFIComposerEmoticonPlugin"
                            ],
                            [
                                "cometUFIComposerPrefillMentionPlugin_plugin$normalization.graphql"
                            ],
                            [
                                "cometUFIComposerPrefillMentionPlugin"
                            ],
                            [
                                "cometUFIComposerAssociateReplyWithParentPlugin_plugin$normalization.graphql"
                            ],
                            [
                                "cometUFIComposerAssociateReplyWithParentPlugin"
                            ],
                            [
                                "cometUFIComposerSetReplyClickedPlugin_plugin$normalization.graphql"
                            ],
                            [
                                "cometUFIComposerSetReplyClickedPlugin"
                            ],
                            [
                                "cometUFIComposerStateSnapshotPlugin_plugin$normalization.graphql"
                            ],
                            [
                                "cometUFIComposerStateSnapshotPlugin"
                            ],
                            [
                                "cometUFIComposerLiveTypingBroadcastPlugin_plugin$normalization.graphql"
                            ],
                            [
                                "cometUFIComposerLiveTypingBroadcastPlugin"
                            ],
                            [
                                "cometUFIComposerCommentCharacterLimitPlugin_plugin$normalization.graphql"
                            ],
                            [
                                "cometUFIComposerCommentCharacterLimitPlugin"
                            ],
                            [
                                "cometUFIComposerWriteToComposerPlugin_plugin$normalization.graphql"
                            ],
                            [
                                "cometUFIComposerWriteToComposerPlugin"
                            ],
                            [
                                "CometUFIGroupCommentActorLink_groupCommentInfo$normalization.graphql"
                            ],
                            [
                                "CometUFIGroupCommentActorLink.react"
                            ],
                            [
                                "CometUFICommentActorUserSignalsRenderer_renderer$normalization.graphql"
                            ],
                            [
                                "CometUFICommentActorUserSignalsRenderer.react"
                            ],
                            [
                                "CometUFICommentTimeStampActionLink_commentActionLink$normalization.graphql"
                            ],
                            [
                                "CometUFICommentTimeStampActionLink.react"
                            ],
                            [
                                "CometUFICommentReactionActionLink_commentActionLink$normalization.graphql"
                            ],
                            [
                                "CometUFICommentReactionActionLink.react"
                            ],
                            [
                                "CometUFICommentReplyActionLink_commentActionLink$normalization.graphql"
                            ],
                            [
                                "CometUFICommentReplyActionLink.react"
                            ],
                            [
                                "CometUFICommentShareActionLinkExperimental_commentActionLink$normalization.graphql"
                            ],
                            [
                                "CometUFICommentShareActionLinkExperimental.react"
                            ],
                            [
                                "CometUFICommentBodyTextWithEntities_textWithEntities$normalization.graphql"
                            ],
                            [
                                "CometUFICommentBodyTextWithEntities.react"
                            ],
                            [
                                "emptyFunction",
                                "thatReturns",
                                [
                                    "RequireDeferredReference"
                                ],
                                [
                                    [
                                        {
                                            "__dr": "CometGenericCommentDisableNotice_commentDisableNotice$normalization.graphql"
                                        },
                                        {
                                            "__dr": "CometGenericCommentDisableNotice.react"
                                        },
                                        {
                                            "__dr": "cometUFIComposerGroupMentionsPlugin_plugin$normalization.graphql"
                                        },
                                        {
                                            "__dr": "cometUFIComposerGroupMentionsPlugin"
                                        },
                                        {
                                            "__dr": "cometUFIComposerAvatarPlugin_plugin$normalization.graphql"
                                        },
                                        {
                                            "__dr": "cometUFIComposerAvatarPlugin"
                                        },
                                        {
                                            "__dr": "cometUFIComposerHashtagPlugin_plugin$normalization.graphql"
                                        },
                                        {
                                            "__dr": "cometUFIComposerHashtagPlugin"
                                        },
                                        {
                                            "__dr": "cometUFIComposerEmojiPlugin_plugin$normalization.graphql"
                                        },
                                        {
                                            "__dr": "cometUFIComposerEmojiPlugin"
                                        },
                                        {
                                            "__dr": "cometUFIComposerMediaUploadPlugin_plugin$normalization.graphql"
                                        },
                                        {
                                            "__dr": "cometUFIComposerMediaUploadPlugin"
                                        },
                                        {
                                            "__dr": "cometUFIComposerGIFPlugin_plugin$normalization.graphql"
                                        },
                                        {
                                            "__dr": "cometUFIComposerGIFPlugin"
                                        },
                                        {
                                            "__dr": "cometUFIComposerStickersPlugin_next_plugin$normalization.graphql"
                                        },
                                        {
                                            "__dr": "cometUFIComposerStickersPlugin.next"
                                        },
                                        {
                                            "__dr": "cometUFIComposerEmoticonPlugin_plugin$normalization.graphql"
                                        },
                                        {
                                            "__dr": "cometUFIComposerEmoticonPlugin"
                                        },
                                        {
                                            "__dr": "cometUFIComposerPrefillMentionPlugin_plugin$normalization.graphql"
                                        },
                                        {
                                            "__dr": "cometUFIComposerPrefillMentionPlugin"
                                        },
                                        {
                                            "__dr": "cometUFIComposerAssociateReplyWithParentPlugin_plugin$normalization.graphql"
                                        },
                                        {
                                            "__dr": "cometUFIComposerAssociateReplyWithParentPlugin"
                                        },
                                        {
                                            "__dr": "cometUFIComposerSetReplyClickedPlugin_plugin$normalization.graphql"
                                        },
                                        {
                                            "__dr": "cometUFIComposerSetReplyClickedPlugin"
                                        },
                                        {
                                            "__dr": "cometUFIComposerStateSnapshotPlugin_plugin$normalization.graphql"
                                        },
                                        {
                                            "__dr": "cometUFIComposerStateSnapshotPlugin"
                                        },
                                        {
                                            "__dr": "cometUFIComposerLiveTypingBroadcastPlugin_plugin$normalization.graphql"
                                        },
                                        {
                                            "__dr": "cometUFIComposerLiveTypingBroadcastPlugin"
                                        },
                                        {
                                            "__dr": "cometUFIComposerCommentCharacterLimitPlugin_plugin$normalization.graphql"
                                        },
                                        {
                                            "__dr": "cometUFIComposerCommentCharacterLimitPlugin"
                                        },
                                        {
                                            "__dr": "cometUFIComposerWriteToComposerPlugin_plugin$normalization.graphql"
                                        },
                                        {
                                            "__dr": "cometUFIComposerWriteToComposerPlugin"
                                        },
                                        {
                                            "__dr": "CometUFIGroupCommentActorLink_groupCommentInfo$normalization.graphql"
                                        },
                                        {
                                            "__dr": "CometUFIGroupCommentActorLink.react"
                                        },
                                        {
                                            "__dr": "CometUFICommentActorUserSignalsRenderer_renderer$normalization.graphql"
                                        },
                                        {
                                            "__dr": "CometUFICommentActorUserSignalsRenderer.react"
                                        },
                                        {
                                            "__dr": "CometUFICommentTimeStampActionLink_commentActionLink$normalization.graphql"
                                        },
                                        {
                                            "__dr": "CometUFICommentTimeStampActionLink.react"
                                        },
                                        {
                                            "__dr": "CometUFICommentReactionActionLink_commentActionLink$normalization.graphql"
                                        },
                                        {
                                            "__dr": "CometUFICommentReactionActionLink.react"
                                        },
                                        {
                                            "__dr": "CometUFICommentReplyActionLink_commentActionLink$normalization.graphql"
                                        },
                                        {
                                            "__dr": "CometUFICommentReplyActionLink.react"
                                        },
                                        {
                                            "__dr": "CometUFICommentShareActionLinkExperimental_commentActionLink$normalization.graphql"
                                        },
                                        {
                                            "__dr": "CometUFICommentShareActionLinkExperimental.react"
                                        },
                                        {
                                            "__dr": "CometUFICommentBodyTextWithEntities_textWithEntities$normalization.graphql"
                                        },
                                        {
                                            "__dr": "CometUFICommentBodyTextWithEntities.react"
                                        }
                                    ]
                                ]
                            ],
                            [
                                "FbtLogging"
                            ],
                            [
                                "IntlQtEventFalcoEvent"
                            ],
                            [
                                "createUpgradedUFI2GroupMentionsComposerPluginForLexical"
                            ],
                            [
                                "MAWMICSafe"
                            ],
                            [
                                "CometSuspenseFalcoEvent"
                            ],
                            [
                                "CometUFIStickersComposerUpgradedPreviewContent.react"
                            ],
                            [
                                "getUpgradedCometHashtagComposerHandler"
                            ],
                            [
                                "getUpgradedCometEmojiComposerHandler"
                            ],
                            [
                                "ContextualConfig"
                            ],
                            [
                                "BladeRunnerClient"
                            ],
                            [
                                "DGWRequestStreamClient"
                            ],
                            [
                                "getUpgradedCometUFIEmoticonsComposerHandler"
                            ],
                            [
                                "UFIODSLogger"
                            ],
                            [
                                "CometUFILiveTypingBroadcastComposerUpgradedPlugin.react"
                            ],
                            [
                                "CometAlertDialogImpl.react"
                            ],
                            [
                                "CometRelayEF"
                            ],
                            [
                                "UserSignalsClientImpressionEventFalcoEvent"
                            ],
                            [
                                "CometUFIFunnelLogger"
                            ],
                            [
                                "CometUfiCommentActionLinksFalcoEvent"
                            ],
                            [
                                "CometGroupsPathingFunnelLogger"
                            ],
                            [
                                "LiveVideoViewerTypedLogger"
                            ],
                            [
                                "CometUFIFeedbackReactMutation"
                            ],
                            [
                                "FbSharingEventFalcoEvent"
                            ],
                            [
                                "ShareMetricsLoggingController"
                            ],
                            [
                                "DelightsTextTriggerPostTappedFalcoEvent"
                            ],
                            [
                                "CometToast.react"
                            ],
                            [
                                "ODS"
                            ],
                            [
                                "MqttLongPollingRunner"
                            ],
                            [
                                "CometExceptionDialog.react"
                            ],
                            [
                                "FDSTooltipDeferredImpl.react"
                            ],
                            [
                                "CometExceptionDialog.react"
                            ],
                            [
                                "KeyframesRenderer"
                            ],
                            [
                                "FBKeyframesLoggedSession"
                            ],
                            [
                                "KeyframesAssetDecoder"
                            ],
                            [
                                "RequireDeferredReference",
                                "unblock",
                                [],
                                [
                                    [
                                        "CometGenericCommentDisableNotice_commentDisableNotice$normalization.graphql",
                                        "CometGenericCommentDisableNotice.react",
                                        "cometUFIComposerGroupMentionsPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerGroupMentionsPlugin",
                                        "cometUFIComposerAvatarPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerAvatarPlugin",
                                        "cometUFIComposerHashtagPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerHashtagPlugin",
                                        "cometUFIComposerEmojiPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerEmojiPlugin",
                                        "cometUFIComposerMediaUploadPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerMediaUploadPlugin",
                                        "cometUFIComposerGIFPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerGIFPlugin",
                                        "cometUFIComposerStickersPlugin_next_plugin$normalization.graphql",
                                        "cometUFIComposerStickersPlugin.next",
                                        "cometUFIComposerEmoticonPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerEmoticonPlugin",
                                        "cometUFIComposerPrefillMentionPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerPrefillMentionPlugin",
                                        "cometUFIComposerAssociateReplyWithParentPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerAssociateReplyWithParentPlugin",
                                        "cometUFIComposerSetReplyClickedPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerSetReplyClickedPlugin",
                                        "cometUFIComposerStateSnapshotPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerStateSnapshotPlugin",
                                        "cometUFIComposerLiveTypingBroadcastPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerLiveTypingBroadcastPlugin",
                                        "cometUFIComposerCommentCharacterLimitPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerCommentCharacterLimitPlugin",
                                        "cometUFIComposerWriteToComposerPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerWriteToComposerPlugin",
                                        "CometUFIGroupCommentActorLink_groupCommentInfo$normalization.graphql",
                                        "CometUFIGroupCommentActorLink.react",
                                        "CometUFICommentActorUserSignalsRenderer_renderer$normalization.graphql",
                                        "CometUFICommentActorUserSignalsRenderer.react",
                                        "CometUFICommentTimeStampActionLink_commentActionLink$normalization.graphql",
                                        "CometUFICommentTimeStampActionLink.react",
                                        "CometUFICommentReactionActionLink_commentActionLink$normalization.graphql",
                                        "CometUFICommentReactionActionLink.react",
                                        "CometUFICommentReplyActionLink_commentActionLink$normalization.graphql",
                                        "CometUFICommentReplyActionLink.react",
                                        "CometUFICommentShareActionLinkExperimental_commentActionLink$normalization.graphql",
                                        "CometUFICommentShareActionLinkExperimental.react",
                                        "CometUFICommentBodyTextWithEntities_textWithEntities$normalization.graphql",
                                        "CometUFICommentBodyTextWithEntities.react",
                                        "CometExceptionDialog.react",
                                        "FDSTooltipDeferredImpl.react"
                                    ],
                                    "sd"
                                ]
                            ],
                            [
                                "RequireDeferredReference",
                                "unblock",
                                [],
                                [
                                    [
                                        "FbtLogging",
                                        "IntlQtEventFalcoEvent",
                                        "createUpgradedUFI2GroupMentionsComposerPluginForLexical",
                                        "MAWMICSafe",
                                        "CometSuspenseFalcoEvent",
                                        "CometUFIStickersComposerUpgradedPreviewContent.react",
                                        "getUpgradedCometHashtagComposerHandler",
                                        "getUpgradedCometEmojiComposerHandler",
                                        "ContextualConfig",
                                        "BladeRunnerClient",
                                        "DGWRequestStreamClient",
                                        "getUpgradedCometUFIEmoticonsComposerHandler",
                                        "UFIODSLogger",
                                        "CometUFILiveTypingBroadcastComposerUpgradedPlugin.react",
                                        "CometAlertDialogImpl.react",
                                        "CometRelayEF",
                                        "UserSignalsClientImpressionEventFalcoEvent",
                                        "CometUFIFunnelLogger",
                                        "CometUfiCommentActionLinksFalcoEvent",
                                        "CometGroupsPathingFunnelLogger",
                                        "LiveVideoViewerTypedLogger",
                                        "CometUFIFeedbackReactMutation",
                                        "FbSharingEventFalcoEvent",
                                        "ShareMetricsLoggingController",
                                        "DelightsTextTriggerPostTappedFalcoEvent",
                                        "CometToast.react",
                                        "ODS",
                                        "MqttLongPollingRunner",
                                        "KeyframesRenderer",
                                        "FBKeyframesLoggedSession",
                                        "KeyframesAssetDecoder"
                                    ],
                                    "sd"
                                ]
                            ],
                            [
                                "RequireDeferredReference",
                                "unblock",
                                [],
                                [
                                    [
                                        "CometGenericCommentDisableNotice_commentDisableNotice$normalization.graphql",
                                        "CometGenericCommentDisableNotice.react",
                                        "cometUFIComposerGroupMentionsPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerGroupMentionsPlugin",
                                        "cometUFIComposerAvatarPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerAvatarPlugin",
                                        "cometUFIComposerHashtagPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerHashtagPlugin",
                                        "cometUFIComposerEmojiPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerEmojiPlugin",
                                        "cometUFIComposerMediaUploadPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerMediaUploadPlugin",
                                        "cometUFIComposerGIFPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerGIFPlugin",
                                        "cometUFIComposerStickersPlugin_next_plugin$normalization.graphql",
                                        "cometUFIComposerStickersPlugin.next",
                                        "cometUFIComposerEmoticonPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerEmoticonPlugin",
                                        "cometUFIComposerPrefillMentionPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerPrefillMentionPlugin",
                                        "cometUFIComposerAssociateReplyWithParentPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerAssociateReplyWithParentPlugin",
                                        "cometUFIComposerSetReplyClickedPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerSetReplyClickedPlugin",
                                        "cometUFIComposerStateSnapshotPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerStateSnapshotPlugin",
                                        "cometUFIComposerLiveTypingBroadcastPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerLiveTypingBroadcastPlugin",
                                        "cometUFIComposerCommentCharacterLimitPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerCommentCharacterLimitPlugin",
                                        "cometUFIComposerWriteToComposerPlugin_plugin$normalization.graphql",
                                        "cometUFIComposerWriteToComposerPlugin",
                                        "CometUFIGroupCommentActorLink_groupCommentInfo$normalization.graphql",
                                        "CometUFIGroupCommentActorLink.react",
                                        "CometUFICommentActorUserSignalsRenderer_renderer$normalization.graphql",
                                        "CometUFICommentActorUserSignalsRenderer.react",
                                        "CometUFICommentTimeStampActionLink_commentActionLink$normalization.graphql",
                                        "CometUFICommentTimeStampActionLink.react",
                                        "CometUFICommentReactionActionLink_commentActionLink$normalization.graphql",
                                        "CometUFICommentReactionActionLink.react",
                                        "CometUFICommentReplyActionLink_commentActionLink$normalization.graphql",
                                        "CometUFICommentReplyActionLink.react",
                                        "CometUFICommentShareActionLinkExperimental_commentActionLink$normalization.graphql",
                                        "CometUFICommentShareActionLinkExperimental.react",
                                        "CometUFICommentBodyTextWithEntities_textWithEntities$normalization.graphql",
                                        "CometUFICommentBodyTextWithEntities.react",
                                        "CometExceptionDialog.react",
                                        "FDSTooltipDeferredImpl.react"
                                    ],
                                    "css"
                                ]
                            ],
                            [
                                "RequireDeferredReference",
                                "unblock",
                                [],
                                [
                                    [
                                        "FbtLogging",
                                        "IntlQtEventFalcoEvent",
                                        "createUpgradedUFI2GroupMentionsComposerPluginForLexical",
                                        "MAWMICSafe",
                                        "CometSuspenseFalcoEvent",
                                        "CometUFIStickersComposerUpgradedPreviewContent.react",
                                        "getUpgradedCometHashtagComposerHandler",
                                        "getUpgradedCometEmojiComposerHandler",
                                        "ContextualConfig",
                                        "BladeRunnerClient",
                                        "DGWRequestStreamClient",
                                        "getUpgradedCometUFIEmoticonsComposerHandler",
                                        "UFIODSLogger",
                                        "CometUFILiveTypingBroadcastComposerUpgradedPlugin.react",
                                        "CometAlertDialogImpl.react",
                                        "CometRelayEF",
                                        "UserSignalsClientImpressionEventFalcoEvent",
                                        "CometUFIFunnelLogger",
                                        "CometUfiCommentActionLinksFalcoEvent",
                                        "CometGroupsPathingFunnelLogger",
                                        "LiveVideoViewerTypedLogger",
                                        "CometUFIFeedbackReactMutation",
                                        "FbSharingEventFalcoEvent",
                                        "ShareMetricsLoggingController",
                                        "DelightsTextTriggerPostTappedFalcoEvent",
                                        "CometToast.react",
                                        "ODS",
                                        "MqttLongPollingRunner",
                                        "KeyframesRenderer",
                                        "FBKeyframesLoggedSession",
                                        "KeyframesAssetDecoder"
                                    ],
                                    "css"
                                ]
                            ]
                        ]
                    },
                    "allResources": [
                        "v39gSxj",
                        "vhKfY5c",
                        "2hPt+8f",
                        "UZfqf8J",
                        "cKZv3P8",
                        "UX5ZaR7",
                        "uLB6aZe",
                        "eJ8EHGb",
                        "QHlvoYy",
                        "4UiubQr",
                        "AdpmZX+",
                        "mbuNvlv",
                        "tytAcfm",
                        "mueC9mU",
                        "zdnyIKV",
                        "nVZGLFA",
                        "7L5r4xF",
                        "w0NV5zs",
                        "19hbtN7",
                        "BOv7jro",
                        "7CxomUC",
                        "I9Os7/3",
                        "ao/gvNJ",
                        "XogzSlm",
                        "p6J0Y88",
                        "x4h+czF"
                    ]
                }
            }
        }
    }
}
```
</details>
