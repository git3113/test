#See https://aka.ms/customizecontainer to learn how to customize your debug container and how Visual Studio uses this Dockerfile to build your images for faster debugging.

# 使用官方的 .NET 6.0 SDK 镜像作为基础镜像
FROM mcr.microsoft.com/dotnet/aspnet:3.1 AS base

 # WORKDIR 镜像的工作目录
WORKDIR /app

 # 暴露端口
EXPOSE 9900
EXPOSE 443

 # 复制文件
COPY . .

 # 定义启动命令
ENTRYPOINT ["dotnet", "webapi.dll"]
