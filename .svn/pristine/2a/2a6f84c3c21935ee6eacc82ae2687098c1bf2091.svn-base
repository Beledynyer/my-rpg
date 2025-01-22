using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using Engine.Models;

namespace Engine.Factories
{
    static internal class QuestFactory
    {
        private static List<Quest> _quests = new List<Quest>();

        static QuestFactory() { 

            List<ItemQuantity> itemsToComplete = new List<ItemQuantity>();
            List<ItemQuantity> rewardItems = new List<ItemQuantity>();

            itemsToComplete.Add(new ItemQuantity(9001, 5));// 5 snakes fangs 
            rewardItems.Add(new ItemQuantity(1002, 1)); // 1 rusty sword

            _quests.Add(new Quest(1,
                "Clear the herb garden",
                "Defeat the snakes in the Herbalist's Garden",
                itemsToComplete,
                25,10,
                rewardItems));
        }

        internal static Quest GetQuestByID(int id)
        {
            return _quests.FirstOrDefault(quest => quest.ID == id);
        }
    }
}
