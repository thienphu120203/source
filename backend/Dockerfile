FROM mcr.microsoft.com/dotnet/sdk:6.0
WORKDIR /app

COPY . .
RUN dotnet restore
#Tạo người dùng không phải là quyền root
#RUN useradd -m ecommerce-fullstack

# Set quyền sỡ hữu của thư mục app cho user mới
#RUN chown -R ecommerce-fullstack:ecommerce-fullstack /app

# Chuyển người dùng sang ecommerce-fullstack 
#USER ecommerce-fullstack


CMD ["dotnet", "run", "--urls", "http://0.0.0.0:5214"]

