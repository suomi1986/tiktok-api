# tiktok-api
 TikTok Full Mobile API, X-Argus, X-Ladon, X-Gorgon, X-Khronos, TTEncrypt, X-Log, Applog tiktok api last version mass account creator of tik tok accounts, tik tok likes, comments, tik tok latest version

## Contact for api : [https://t.me/suomi1986](https://t.me/suomi1986)


ef home_list(self, user_data={}):
        url = self.api_url + "aweme/v1/feed/?count=20&offset=0&max_cursor=0&type=0&is_cold_start=1&pull_type=1&" + self.helper.query(
            self.helper.default_variable(self.global_variable))
        if (user_data.__len__() > 0):
            data = self.helper.request_get(self, url, session=self.active_user['cookies'])
        else:
            data = self.helper.request_get(self, url)
        return data.json()

    def search_user(self, text='teamtolga', session={}):
        url = self.api_url + "aweme/v1/discover/search/?cursor=0&keyword=" + text + "&count=10&type=1&hot_search=0&" + self.helper.query(
            self.helper.default_variable(self.global_variable))
        if (session.__len__() > 0):
            data = self.helper.request_get(self, url, session=session)
        else:
            data = self.helper.request_get(self, url)
        return data.json()

    def like_post(self, aweme_id=1, type='1', session={}):
        url = self.api_url + "aweme/v1/commit/item/digg/?aweme_id=" + aweme_id + "&type=" + type + "&retry_type=no_retry&from=3&" + self.helper.query(
            self.helper.default_variable(self.global_variable))
        data = self.helper.request_get(self, url, session=session)
        return data.json()



1. login to the user by email and username
2. register new device
3. receive information of the user through user_id
4. receive information about your authorized profile
5. get list of user's subscribers
6. get list of user's subscriptions
7. receive user posts (publications)
8. receive comments for posts
9. like comments
10. like posts
11. subscribe to user
12. search
13. search hashtags
14. search post hashtags
15. search users
16. Download Post By Video Id
17. Download tiktok video without watermark


## Contact for api : [https://t.me/suomi1986](https://t.me/suomi1986)
