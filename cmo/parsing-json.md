``` java
JSONObject jObj = new JSONObject(jsonStr);
JSONArray jsonArry = jObj.getJSONArray("users");
for(int i=0;i<jsonArry.length();i++){
    HashMap<String,String> user = new HashMap<>();
    JSONObject obj = jsonArry.getJSONObject(i);
    user.put("name",obj.getString("name"));
    user.put("designation",obj.getString("designation"));
    user.put("location",obj.getString("location"));
    userList.add(user);
}
