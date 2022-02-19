 builder.Entity<User>().HasData(
                new User
                {
                    Id ="1023",
                    Email = "ali.xudiyev98@gmail.com",
                    FirstName ="Əli",
                    LastName ="Xudiyev",
                    Address ="Azərbaycan, Cəlilabad, Alar",
                    PhoneNumber ="+994-55-305-32-32",
                    UserName ="ali.xudiyev98@gmail.com",
                    ConcurrencyStamp ="sdchsuicmkms",
                    EmailConfirmed =true,
                    NormalizedEmail="ALI.XUDIYEV98@GMAIL.COM",
                    PhoneNumberConfirmed =true, 
                    LockoutEnabled=true,
                    NormalizedUserName= "ALI.XUDIYEV98@GMAIL.COM",
                    TwoFactorEnabled=true,
                    AccessFailedCount=1,
                    LockoutEnd=DateTime.Now,
                    PasswordHash=null,
                    SecurityStamp=null,
                });

            builder.Entity<IdentityRole>().HasData(
                new IdentityRole
                {
                    Id ="abs21",
                    Name ="Admin",
                    NormalizedName="ADMIN",
                    ConcurrencyStamp="sdxjwdxjmskm"
                }
                );
            builder.Entity<IdentityUserRole<string>>().HasData(
                new IdentityUserRole<string>
                {
                    RoleId= "abs21",
                    UserId="1023"
                });
