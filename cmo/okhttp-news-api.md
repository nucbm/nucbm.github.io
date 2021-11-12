read more:
https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/about-writing-and-formatting-on-github


``` Java
OkHttpClient client = new OkHttpClient();

Request request = new Request.Builder()
	.url("https://bravenewcoin.p.rapidapi.com/market-cap?assetId=%3CREQUIRED%3E")
	.get()
	.addHeader("authorization", "Bearer <append token here>")
	.addHeader("x-rapidapi-host", "bravenewcoin.p.rapidapi.com")
	.addHeader("x-rapidapi-key", "bbb9713fb5msh23325af22cf06efp1eee63jsn0222de296865")
	.build();

Response response = client.newCall(request).execute();
