using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Engine.Models
{
    public class Weapon :GameItem
    {
        public int MaximumDamage { get; set; }
        public int MinimumDamage { get; set; }

        public Weapon(int itemTypeID, String name, int price, int minimumDamage,int maximumDamage) : base(itemTypeID, name, price) { 
            MaximumDamage = maximumDamage;
            MinimumDamage = minimumDamage;
        }

        public new Weapon Clone()
        {
            return new Weapon(ItemTypeID, Name, Price, MinimumDamage,MaximumDamage);
        }
    }
}
