//初始化
<?xml version="1.0" encoding="utf-8"?>
<com.zhjk.admin.mylibrary.MultipleStatusView  xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/multipleStatusView"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@color/backgroundColor"
    app:emptyView="@layout/layout_empty_view"
    app:errorView="@layout/layout_error_view"
    app:loadingView="@layout/layout_loading_view"
    app:noNetworkView="@layout/layout_network_view">
</com.zhjk.admin.mylibrary.MultipleStatusView >
//调用 加载
mLayoutStatusView?.showLoading()

// 加载完成 展示页面
  mLayoutStatusView?.showContent()
  
//加载网络错误 
mLayoutStatusView?.showNoNetwork()

//其他错误页面 
mLayoutStatusView?.showError()
