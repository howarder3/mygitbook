# C++ json

* task.mmParcel = clip.HasMember("mmParcel") ? clip\["mmParcel"].GetString() : "{}";
* task.duration = clip.HasMember("duration") ? clip\["duration"].GetInt() : 0;
* task.userId = clip.HasMember("userUid") ? clip\["userUid"].GetString() : "";
* task.plan = clip.HasMember("plan") ? clip\["plan"].GetInt() : 1;
* task.startTime = clip.HasMember("startTime") ? clip\["startTime"].GetInt64() : 0;
